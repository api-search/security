---
api_key_in: []
auth_types:
- proprietary-account
- hardware-otp
description: ''
kind: authentication
layout: security
method: searched
name: Teranet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teranet secures its APIs with proprietary-account and hardware-otp across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Teranet
provider_slug: teranet
scheme_count: 4
schemes:
- description: Account Name plus User Name plus password. The Account Name identifies the licensed organization (a law firm or vendor); the User Name identifies the individual within it. Both are issued by Teranet at account setup, not chosen self-serve.
  factors:
  - account name
  - user name
  - password
  name: Teraview account
  source: https://www.teraview.ca/en/teraview-training-environment/
  type: proprietary
- description: A second factor supplied by an RSA token with a user-set PIN, required for production Teraview access. In the published training environment any six digits are accepted as the PIN.
  name: RSA hardware token
  source: https://www.teraview.ca/en/teraview-training-environment/
  type: otp
- description: 'Announced 2026-07-20 as an enhancement to the Teraview sign-in experience: email-based login replacing the Account Name / User Name pair, with Multi-Factor Authentication enhancements. Supersedes the RSA-token model over time.'
  name: Email-based sign-in with enhanced MFA
  source: https://www.teraview.ca/en/2026/
  status: rolling-out
  type: proprietary
- applies_to: teranet:teranet-connect
  contact: info@teranet.ca
  description: Teranet Connect is described by Teranet as providing "secure access" over XML and Web services interfaces, but the credential model is not documented publicly. Access is granted only under a licence agreement negotiated with a Teranet account manager, and transactions are billed against the licensee's existing Teraview Deposit Account — meaning the Deposit Account is the effective identity and billing principal for API calls.
  name: Teranet Connect licensed integration
  self_serve: false
  source: https://www.teranet.ca/registry-solutions/province-of-ontario/teranet-connect/
  type: proprietary
slug: teranet-authentication
source_filename: teranet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://www.teraview.ca/en/teraview-training-environment/\ndocs: https://www.teraview.ca/en/become-a-teraview-user/\nsummary:\n  types:\n  - proprietary-account\n  - hardware-otp\n  api_key_in: []\n  oauth2_flows: []\n  openapi_derived: false\n  note: >-\n    Derived mechanically from OpenAPI is impossible here — Teranet publishes no OpenAPI, Swagger or\n    any other machine-readable contract, so this profile is searched from documentation only. There\n    are no securitySchemes to aggregate.\nmodel: >-\n  Teranet authenticates people and licensed organizations, not applications. Access to every\n  Teranet surface — Teraview, OnLand, GeoWarehouse, Teranet eXpress and the Teranet Connect API —\n  is gated on a commercial account that must be established before any credential exists. There is\n  no self-serve credential issuance, no API key console, no OAuth authorization server, no OIDC\n  discovery document and no public token\
  \ endpoint. This is the defining characteristic of Teranet's\n  API posture: the authentication barrier is contractual before it is technical.\nschemes:\n- name: Teraview account\n  type: proprietary\n  description: >-\n    Account Name plus User Name plus password. The Account Name identifies the licensed\n    organization (a law firm or vendor); the User Name identifies the individual within it. Both\n    are issued by Teranet at account setup, not chosen self-serve.\n  factors:\n  - account name\n  - user name\n  - password\n  source: https://www.teraview.ca/en/teraview-training-environment/\n- name: RSA hardware token\n  type: otp\n  description: >-\n    A second factor supplied by an RSA token with a user-set PIN, required for production\n    Teraview access. In the published training environment any six digits are accepted as the PIN.\n  source: https://www.teraview.ca/en/teraview-training-environment/\n- name: Email-based sign-in with enhanced MFA\n  type: proprietary\n  status:\
  \ rolling-out\n  description: >-\n    Announced 2026-07-20 as an enhancement to the Teraview sign-in experience: email-based login\n    replacing the Account Name / User Name pair, with Multi-Factor Authentication enhancements.\n    Supersedes the RSA-token model over time.\n  source: https://www.teraview.ca/en/2026/\n- name: Teranet Connect licensed integration\n  type: proprietary\n  applies_to: teranet:teranet-connect\n  description: >-\n    Teranet Connect is described by Teranet as providing \"secure access\" over XML and Web services\n    interfaces, but the credential model is not documented publicly. Access is granted only under a\n    licence agreement negotiated with a Teranet account manager, and transactions are billed\n    against the licensee's existing Teraview Deposit Account — meaning the Deposit Account is the\n    effective identity and billing principal for API calls.\n  self_serve: false\n  contact: info@teranet.ca\n  source: https://www.teranet.ca/registry-solutions/province-of-ontario/teranet-connect/\n\
  absent:\n  oauth2: true\n  openid_connect: true\n  api_keys: true\n  mutual_tls: unknown\n  jwt: unknown\n  note: >-\n    \"absent\" here means not publicly documented. Teranet may operate any of these behind the\n    licence gate; nothing in the public record evidences them, and nothing has been assumed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teranet/refs/heads/main/authentication/teranet-authentication.yml
summary_line: proprietary-account/hardware-otp · 4 schemes
tags:
- Real-Estate
- Canada
- Land Registry
- Title
- Conveyancing
- Property Data
- Valuation
- AVM
- PropTech
- Government
- Geospatial
---
