---
api_key_in:
- header
api_specs:
- filename: broadlume-bms-openapi.yml
  format: yaml
  label: Broadlume BMS API
  slug: bms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadlume/refs/heads/main/openapi/broadlume-bms-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Broadlume Authentication
name_suffix: Authentication
oauth_flows: []
overview: Broadlume secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Broadlume
provider_slug: broadlume
scheme_count: 2
schemes:
- description: API key issued by Broadlume, required on every request including the token endpoint and the unauthenticated version endpoint.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/broadlume-bms-openapi.yml
  - https://developer.broadlume.com/bms/authentication
  type: apiKey
- description: User session token obtained from POST /{alias}/token. Required on every operation except GET /{alias}/version and POST /{alias}/token.
  in: header
  name: sessionToken
  parameter: token
  sources:
  - openapi/broadlume-bms-openapi.yml
  - https://developer.broadlume.com/bms/authentication
  type: apiKey
slug: broadlume-authentication
source_filename: broadlume-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/broadlume-bms-openapi.yml\ndocs: https://developer.broadlume.com/bms/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: two-factor header auth — a static Broadlume-issued API key plus a per-user session token\n  oauth2: false\n  oauth2_flows: []\n  note: Broadlume BMS uses no OAuth 2.0 or OpenID Connect. Every request carries two headers, and the\n    session token is minted by a dedicated token endpoint rather than by a standards-based authorization\n    server.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued by Broadlume, required on every request including the token endpoint and\n    the unauthenticated version endpoint.\n  sources:\n  - openapi/broadlume-bms-openapi.yml\n  - https://developer.broadlume.com/bms/authentication\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: token\n  description: User\
  \ session token obtained from POST /{alias}/token. Required on every operation except\n    GET /{alias}/version and POST /{alias}/token.\n  sources:\n  - openapi/broadlume-bms-openapi.yml\n  - https://developer.broadlume.com/bms/authentication\nflow:\n  step_1: GET /{alias}/version — reachable with only x-api-key; returns the deployed API version.\n  step_2: POST /{alias}/token with {username, password, granttype} and the x-api-key header; returns\n    TOKEN plus the COMPANIES the user may access.\n  step_3: Send both x-api-key and token headers on every subsequent call.\n  step_4: GET /{alias}/token (keepalive) to validate a token and reset its idle timer.\n  step_5: DELETE /{alias}/token to end the session; required to reissue an application token.\ngrant_types:\n- name: client\n  default: true\n  description: Times out after a server-specified idle period (documented default 5 minutes). Any API\n    call refreshes the last-active time, so a keepalive call is only needed while idle.\
  \ Once expired the\n    token is invalid and a new one must be minted.\n- name: application\n  default: false\n  description: Long-term token for API-to-API transactions. Does not time out provided it is used within\n    a year of creation. A DELETE on the token endpoint is required to reset the issued key.\ncredentials:\n  username:\n    max_length: 8\n    required: true\n  password:\n    max_length: 8\n    required: true\n  note: The documented credential fields are capped at 8 characters each, reflecting the underlying\n    RollMaster ERP user model.\ntenancy:\n  alias: Path segment on every operation — the client id identifying the Broadlume BMS tenant.\n  company: Query/body parameter, 2 characters; scopes 203 of 256 documented operations.\n  branch: Query/body parameter, 2 characters; scopes 86 operations. Active branches are set per session\n    via POST /{alias}/changebranch, and subsequent queries filter to the active branch list.\nsession_limits:\n  endpoint: GET /{alias}/sessioncount\n\
  \  returns:\n  - SESSIONCOUNT\n  - LIMIT\n  note: Concurrent sessions are capped per tenant. The limit value is discoverable at runtime but is not\n    published as a number in the documentation.\nonboarding:\n  public_self_service: false\n  note: The reference is public, but the x-api-key, the alias and user credentials are issued by\n    Broadlume to BMS customers; there is no self-service signup or published key-request form.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadlume/refs/heads/main/authentication/broadlume-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Flooring
- Retail
- Marketing
- Websites
- Business Software
- Home Improvement
- ERP
- Inventory
- Point-of-Sale
- Accounting
- Order Management
---
