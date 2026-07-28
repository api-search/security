---
api_key_in: []
auth_types:
- saml2
description: ''
kind: authentication
layout: security
method: searched
name: Nova Scotia Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nova Scotia Power secures its APIs with saml2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nova Scotia Power
provider_slug: nova-scotia-power
scheme_count: 1
schemes:
- description: Browser-based SAML 2.0 single sign-on for Nova Scotia Power customers. This is human identity for a self-service portal, not an API authorization scheme — it issues a browser session, not a token a third party can hold.
  hsts: max-age=31536000; includeSubDomains; preload (accounts and myaccount)
  identity_provider: https://accounts.nspower.ca/
  identity_provider_vendor: LoginRadius. accounts.nspower.ca resolves via the CNAME chain novascotiapower.hub.loginradius.com -> hub.loginradius.com -> td.loginradius.com.
  name: nspower-customer-saml-sso
  observed_behaviour: Every path requested on greenbutton.nspower.ca — including nonexistent ones and the canonical ESPI resource paths — 302s to https://accounts.nspower.ca/service/saml/idp/login?appName=greenbutton&SAMLRequest=... with a RelayState.
  service_providers:
  - https://greenbutton.nspower.ca/
  - https://myaccount.nspower.ca/
  source: https://greenbutton.nspower.ca/
  type: saml2
slug: nova-scotia-power-authentication
source_filename: nova-scotia-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.nspower.ca/cleanandgreen/innovation\ndocs:\n- https://www.nspower.ca/cleanandgreen/innovation\n- https://greenbutton.nspower.ca/\n- https://accounts.nspower.ca/\nnote: >-\n  Nova Scotia Power publishes no API and therefore no API authentication. This\n  artifact records what actually gates its data surfaces, observed live on\n  2026-07-27, so the absence is documented rather than silent. There is no OpenAPI\n  or discovery document to derive securitySchemes from — derive-authentication.py\n  has no spec to read. Everything below was observed by following redirects and\n  probing discovery paths; nothing is inferred from what the standard would imply.\nsummary:\n  types:\n  - saml2\n  api_auth_available: false\n  oauth2_flows: []\n  api_key_in: []\n  discovery_document: false\n  self_serve_credentials: false\n  third_party_access: closed\nschemes:\n- name: nspower-customer-saml-sso\n  type: saml2\n  description:\
  \ >-\n    Browser-based SAML 2.0 single sign-on for Nova Scotia Power customers. This is\n    human identity for a self-service portal, not an API authorization scheme — it\n    issues a browser session, not a token a third party can hold.\n  identity_provider: https://accounts.nspower.ca/\n  identity_provider_vendor: >-\n    LoginRadius. accounts.nspower.ca resolves via the CNAME chain\n    novascotiapower.hub.loginradius.com -> hub.loginradius.com -> td.loginradius.com.\n  service_providers:\n  - https://greenbutton.nspower.ca/\n  - https://myaccount.nspower.ca/\n  observed_behaviour: >-\n    Every path requested on greenbutton.nspower.ca — including nonexistent ones and\n    the canonical ESPI resource paths — 302s to\n    https://accounts.nspower.ca/service/saml/idp/login?appName=greenbutton&SAMLRequest=...\n    with a RelayState.\n  hsts: 'max-age=31536000; includeSubDomains; preload (accounts and myaccount)'\n  source: https://greenbutton.nspower.ca/\nnot_published:\n  oauth2: >-\n\
  \    None. The Green Button Connect My Data profile — the OAuth 2.0 authorization\n    code flow that would let a customer grant a third-party application access to\n    their interval data — is not certified and not deployed.\n    https://greenbutton.nspower.ca/oauth/authorize and\n    /DataCustodian/oauth/authorize both 302 to the SAML IdP.\n  api_keys: None published. There is no key issuance surface of any kind.\n  mtls: None published.\n  client_registration: >-\n    None. Nova Scotia Power's Innovation page states \"Our Green Button Marketplace\n    is currently closed\", and the linked third-party registration form at\n    /cleanandgreen/innovation/green-button-registration-form returns HTTP 404 — the\n    only published route for a developer to request access is a dead link.\n  scopes: >-\n    No scope surface exists. NAESB ESPI function-block scopes (FB=...) would only\n    appear on a Connect My Data authorization request; there is no such request to\n    observe, so no scopes/\
  \ artifact is emitted.\ndiscovery:\n  openid_configuration:\n  - url: https://accounts.nspower.ca/.well-known/openid-configuration\n    status: 404\n    body: '{\"ErrorCode\":404,\"Message\":\"Resource not found\",\"Description\":\"Sorry, the resource you were looking for was not found.\"}'\n  - url: https://myaccount.nspower.ca/.well-known/openid-configuration\n    status: 404\n  - url: https://www.nspower.ca/.well-known/openid-configuration\n    status: 404\n  oauth_authorization_server:\n  - url: https://www.nspower.ca/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://accounts.nspower.ca/.well-known/oauth-authorization-server\n    status: 404\n  oauth_protected_resource:\n  - url: https://www.nspower.ca/.well-known/oauth-protected-resource\n    status: 404\naccess_gate:\n  self_serve: false\n  gate: customer-account-required\n  developer_route: none\n  steps:\n  - >-\n    To read your OWN data: create a Nova Scotia Power MyAccount, authenticate\n    through accounts.nspower.ca\
  \ (SAML SSO), and download usage from\n    greenbutton.nspower.ca or myaccount.nspower.ca. This is Download My Data — a\n    human download, not a programmatic interface.\n  - >-\n    To read a CUSTOMER's data as a third party: there is no route. The Green Button\n    Marketplace is closed and its registration form 404s.\n  - >-\n    To read MARKET data: nothing at all — https://www.nspower.ca/oasis serves CSV,\n    HTM and PDF anonymously with no login and no licence click-through.\n  contact: null\n  contact_note: >-\n    No developer, integration or Green Button contact address is published. The only\n    published channel is general customer service at\n    https://www.nspower.ca/customer-service.\nopen_data_auth:\n  surface: https://www.nspower.ca/oasis\n  authentication: none\n  note: >-\n    OASIS monthly reports, system reports and hosting-capacity files are served\n    anonymously over HTTPS as bulk files. Verified anonymously: the 2025 NS-NB tie\n    monthly report CSV returned\
  \ HTTP 200, 253,453 bytes. The transactional\n    reservation node is separate, hosted by OATI at https://www.oasis.oati.com/ and\n    marked \"Secure Site/Registration Required\".\nrelated:\n- conformance/nova-scotia-power-conformance.yml\n- conventions/nova-scotia-power-conventions.yml\n- lifecycle/nova-scotia-power-lifecycle.yml\n- well-known/nova-scotia-power-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-scotia-power/refs/heads/main/authentication/nova-scotia-power-authentication.yml
summary_line: saml2 · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Energy Retailer
- Green Button
- Smart Metering
- Grid
- Renewables
- Solar
- EV Charging
- Energy Markets
- Regulation
---
