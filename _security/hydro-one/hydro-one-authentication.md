---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Hydro One Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hydro One secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hydro One
provider_slug: hydro-one
scheme_count: 2
schemes:
- authorization_surface: https://www.hydroone.com/green-button-cmd-home
  authorization_url: not published
  credential_issuance: '"The information to assist with the connectivity testing will be provided, including Client ID, Client Secret, Test Accounts, URI(s)." Credentials and URIs are issued privately by a Hydro One account executive during onboarding on the HONI third-party portal — none are published.'
  description: NAESB ESPI (Green Button Connect My Data) OAuth 2.0 authorization code grant. The customer is redirected from the third-party vendor's application to Hydro One, authenticates with Hydro One, and consents to release of their energy data; the vendor then exchanges the authorization code for an access token and retrieves ESPI XML from the CMD resource endpoints.
  flow: authorizationCode
  name: green-button-cmd-oauth2
  resource_base_uri: not published
  scope_syntax: FB=<function block ids separated by underscores>;historyLength=<seconds>
  scopes_artifact: scopes/hydro-one-scopes.yml
  source: https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions
  token_url: not published
  type: oauth2
- certificate_authority: HONI-supported CA
  description: Ongoing Conditions of Participation require the vendor to "exchange with HONI and maintain unexpired, unrevoked RSA certificates with a public key length of at least 2048 bits issued by a HONI supported Certificate Authority" and to "implement Transport Layer Security for all exchanges with HONI."
  minimum_key_length: 2048
  name: mutual-certificate-exchange
  source: https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions
  type: mutualTLS
slug: hydro-one-authentication
source_filename: hydro-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions\ndocs:\n- https://www.hydroone.com/saving-money-and-energy/green-button/third-party-apps\n- https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions\n- https://www.hydroone.com/green-button-cmd-home\nnote: >-\n  Derived from Hydro One's published Green Button third-party documentation and\n  terms, and from the live Connect My Data authorization surface. Hydro One\n  publishes no OpenAPI, no endpoint reference, and no OAuth discovery document,\n  so no securitySchemes could be derived mechanically from a specification.\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  discovery_document: false\n  self_serve_credentials: false\nschemes:\n- name: green-button-cmd-oauth2\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n\
  \    NAESB ESPI (Green Button Connect My Data) OAuth 2.0 authorization code grant.\n    The customer is redirected from the third-party vendor's application to Hydro\n    One, authenticates with Hydro One, and consents to release of their energy\n    data; the vendor then exchanges the authorization code for an access token and\n    retrieves ESPI XML from the CMD resource endpoints.\n  authorization_surface: https://www.hydroone.com/green-button-cmd-home\n  authorization_url: not published\n  token_url: not published\n  resource_base_uri: not published\n  scope_syntax: 'FB=<function block ids separated by underscores>;historyLength=<seconds>'\n  scopes_artifact: scopes/hydro-one-scopes.yml\n  credential_issuance: >-\n    \"The information to assist with the connectivity testing will be provided,\n    including Client ID, Client Secret, Test Accounts, URI(s).\" Credentials and\n    URIs are issued privately by a Hydro One account executive during onboarding\n    on the HONI third-party\
  \ portal — none are published.\n  source: https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions\n- name: mutual-certificate-exchange\n  type: mutualTLS\n  description: >-\n    Ongoing Conditions of Participation require the vendor to \"exchange with HONI\n    and maintain unexpired, unrevoked RSA certificates with a public key length of\n    at least 2048 bits issued by a HONI supported Certificate Authority\" and to\n    \"implement Transport Layer Security for all exchanges with HONI.\"\n  minimum_key_length: 2048\n  certificate_authority: HONI-supported CA\n  source: https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions\ncustomer_consent:\n  initiated_by: customer, from the third-party vendor's site or app\n  authentication_at: Hydro One (customer authenticates with the utility, not the vendor)\n  vendor_may_authorize_on_behalf_of_customer: false\n  vendor_may_authorize_note: >-\n    \"Can a vendor submit\
  \ an authorization on behalf of a customer? No. Customers\n    must make their own online authorizations through one of the available methods\n    and authenticate with the utility before a security token can be exchanged and\n    data shared.\"\n  duration: indefinite while the vendor remains authorized\n  revocation: customer may revoke access at any time\n  suspension: >-\n    HONI may suspend vendor access without notice where ordered by the Ontario\n    Energy Board or on reasonable evidence of material breach.\naccess_gate:\n  self_serve: false\n  gate: application-approval\n  steps:\n  - Accept the Green Button Third-Party Terms and Conditions.\n  - Register on the HONI third-party portal via the onboarding application form.\n  - Receive Client ID, Client Secret, Test Accounts and URI(s) privately from a HONI account executive.\n  - Complete connectivity testing within 90 days (status moves Ready To Test -> Approved).\n  - Exchange and maintain RSA 2048-bit certificates; implement\
  \ TLS on all exchanges with HONI.\n  contact: greenbutton@HydroOne.com\ndiscovery:\n  openid_configuration: 'https://www.hydroone.com/.well-known/openid-configuration — HTTP 500 (no discovery document)'\n  oauth_authorization_server: 'https://www.hydroone.com/.well-known/oauth-authorization-server — HTTP 500 (no discovery document)'\n  oauth_protected_resource: 'https://www.hydroone.com/.well-known/oauth-protected-resource — HTTP 500 (no discovery document)'\nrelated:\n- scopes/hydro-one-scopes.yml\n- conventions/hydro-one-conventions.yml\n- conformance/hydro-one-conformance.yml\n- sandbox/hydro-one-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-one/refs/heads/main/authentication/hydro-one-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Smart Metering
- Green Button
- Energy Data
- Transmission
- Distribution
---
