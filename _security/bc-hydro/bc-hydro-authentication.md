---
api_key_in: []
auth_types:
- session-sso
description: ''
kind: authentication
layout: security
method: searched
name: Bc Hydro Authentication
name_suffix: Authentication
oauth_flows: []
overview: BC Hydro secures its APIs with session-sso across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BC Hydro
provider_slug: bc-hydro
scheme_count: 1
schemes:
- authorization_endpoint: https://app.bchydro.com/sso/UI/Login
  bearer_tokens_issued_to_third_parties: false
  description: Customer-portal single sign-on. https://www.bchydro.com/login (HTTP 200) redirects to a ForgeRock/OpenAM-style endpoint at https://app.bchydro.com/sso/UI/Login carrying goto, nonce and realm=bch-ps parameters, and lands the authenticated customer on the BCHCustomerPortal. The same path is reached from https://app.bchydro.com/BCHCustomerPortal/web/login.html. The session, not a token, is what authorizes the subsequent CSV / Green Button XML download.
  login_url: https://www.bchydro.com/login
  name: myhydro-customer-sso
  realm: bch-ps
  source: observed redirect chain, 2026-07-27
  token_endpoint: null
  type: session-sso
slug: bc-hydro-authentication
source_filename: bc-hydro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.bchydro.com/login\ndocs:\n- https://www.bchydro.com/login\n- https://app.bchydro.com/accounts-billing/bill-payment/view-bill.html\n- https://app.bchydro.com/accounts-billing/rates-energy-use/access-load-data.html\nnote: >-\n  BC Hydro publishes no OpenAPI, no OAuth discovery document and no third-party\n  authorization surface, so no securityScheme could be derived mechanically from a\n  specification. What exists is a customer-portal session SSO that gates a\n  human-initiated file download; it is recorded here as the real auth model, not\n  as an API authentication contract. Nothing in this file was inferred from a\n  standard BC Hydro does not implement.\nsummary:\n  types:\n  - session-sso\n  oauth2_flows: []\n  api_key_in: []\n  discovery_document: false\n  self_serve_credentials: false\n  third_party_access: false\nschemes:\n- name: myhydro-customer-sso\n  type: session-sso\n  description: >-\n    Customer-portal\
  \ single sign-on. https://www.bchydro.com/login (HTTP 200)\n    redirects to a ForgeRock/OpenAM-style endpoint at\n    https://app.bchydro.com/sso/UI/Login carrying goto, nonce and realm=bch-ps\n    parameters, and lands the authenticated customer on the BCHCustomerPortal.\n    The same path is reached from\n    https://app.bchydro.com/BCHCustomerPortal/web/login.html. The session, not a\n    token, is what authorizes the subsequent CSV / Green Button XML download.\n  login_url: https://www.bchydro.com/login\n  authorization_endpoint: https://app.bchydro.com/sso/UI/Login\n  realm: bch-ps\n  token_endpoint: null\n  bearer_tokens_issued_to_third_parties: false\n  source: observed redirect chain, 2026-07-27\naccess_gate:\n  self_serve: false\n  gate: customer-account-required\n  steps:\n  - Be a BC Hydro account holder (BC Hydro is the monopoly electricity retailer in its service area).\n  - Register for a MyHydro account.\n  - Sign in at https://www.bchydro.com/login.\n  - 'Download your\
  \ own data manually: a CSV or Green Button XML file of metered\n    electricity use from the billing pages, available through the previous day,\n    up to three years of history.'\n  - >-\n    Large, multi-unit or strata customers may instead submit a peak-load-data\n    request form and receive a report; contractors and consultants may request on\n    a customer's behalf, subject to BC Hydro demanding \"authentication questions\n    or proof\" of authorization.\n  developer_signup: null\n  api_keys_issued: false\n  oauth_client_registration: false\n  accreditation_path: null\nthird_party_access:\n  available: false\n  detail: >-\n    No third party can obtain a BC Hydro customer's usage or billing data\n    programmatically. There is no Green Button Connect My Data, no OAuth 2.0\n    authorization or token endpoint, no vendor onboarding form, no data-recipient\n    terms and no published resource base URI. This is the structural difference\n    from a mandated Ontario distributor such\
  \ as Hydro One, which O. Reg. 633/21\n    compels to run a live CMD OAuth surface — no equivalent regulation binds BC\n    Hydro.\nmachine_hosts:\n  api.bchydro.com: >-\n    Resolves to a BC Hydro-owned IP and presents a valid Entrust OV certificate\n    issued to British Columbia Hydro and Power Authority, but rejects TLS 1.2 and\n    returns nothing over TLS 1.3 to any anonymous HTTP request. No authentication\n    scheme is advertised (no WWW-Authenticate, no client-certificate request, no\n    ALPN). Whatever it fronts is not anonymously discoverable.\ndiscovery:\n  openid_configuration: 'https://app.bchydro.com/.well-known/openid-configuration — HTTP 200 soft 404 (redirects to /siteinfo/404.html); no discovery document'\n  oauth_authorization_server: 'https://www.bchydro.com/.well-known/oauth-authorization-server — HTTP 200 soft 404; no discovery document'\n  oauth_protected_resource: 'https://www.bchydro.com/.well-known/oauth-protected-resource — HTTP 200 soft 404; no discovery document'\n\
  related:\n- conformance/bc-hydro-conformance.yml\n- conventions/bc-hydro-conventions.yml\n- lifecycle/bc-hydro-lifecycle.yml\n- well-known/bc-hydro-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bc-hydro/refs/heads/main/authentication/bc-hydro-authentication.yml
summary_line: session-sso · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Crown Corporation
- Hydroelectric
- Renewables
- Grid
- Transmission
- Distribution
- Smart Metering
- Green Button
- Energy Data
- EV Charging
---
