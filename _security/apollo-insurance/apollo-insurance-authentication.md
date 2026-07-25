---
api_key_in:
- header
api_specs:
- filename: apollo-insurance-affiliates.yml
  format: yaml
  label: APOLLO Affiliates API
  slug: apollo-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates.yml
- filename: apollo-insurance-affiliates-legacy.yml
  format: yaml
  label: APOLLO Public API - Affiliates
  slug: apollo-public-api-affiliates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates-legacy.yml
- filename: apollo-insurance-covertrack.yml
  format: yaml
  label: APOLLO CoverTrack API
  slug: apollo-covertrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-covertrack.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apollo Insurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: APOLLO Insurance secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APOLLO Insurance
provider_slug: apollo-insurance
scheme_count: 3
schemes:
- applied: 'global security requirement: security: [{apiKeyAuth: []}]'
  declared: true
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/apollo-insurance-affiliates.yml
  type: apiKey
- applied: Present as an explicit header parameter on every path, but with no components.securitySchemes block and no security requirement. On the callback specification it is described as "API Key (recommended)" rather than required.
  declared: false
  in: header
  name: x-api-key (undeclared)
  parameter: x-api-key
  sources:
  - openapi/apollo-insurance-covertrack.yml
  type: apiKey
- applied: The superseded affiliate generation declares an x-api-key header parameter on each operation but no securitySchemes and no security requirement.
  declared: false
  name: none declared
  sources:
  - openapi/apollo-insurance-affiliates-legacy.yml
  type: null
slug: apollo-insurance-authentication
source_filename: apollo-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/apollo-insurance-affiliates.yml, openapi/apollo-insurance-covertrack.yml\ndocs: https://docs.apollocover.com/docs/public-affiliate-api/27500feeac1b7-introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  self_serve: false\n  model: >-\n    A single static API key header, hand-issued by APOLLO to affiliates and property-manager\n    partners, with all authorization carried in path identifiers rather than in the token. No\n    OAuth, no OIDC, no scopes, no token exchange, no rotation endpoint and no /.well-known/\n    discovery on any host.\n\npublished_guidance: >-\n  \"All endpoints require an `affiliateId` (provided by your APOLLO Contact) and a\n  `insuranceType` in the path. Currently only the `tenant` insurance type is available. All\n  endpoints require a `x-api-key` security token in the header. This token will be provided to\n  you by APOLLO.\"\n\nschemes:\n- name: apiKeyAuth\n\
  \  type: apiKey\n  in: header\n  parameter: x-api-key\n  declared: true\n  applied: 'global security requirement: security: [{apiKeyAuth: []}]'\n  sources:\n  - openapi/apollo-insurance-affiliates.yml\n- name: x-api-key (undeclared)\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  declared: false\n  applied: >-\n    Present as an explicit header parameter on every path, but with no components.securitySchemes\n    block and no security requirement. On the callback specification it is described as\n    \"API Key (recommended)\" rather than required.\n  sources:\n  - openapi/apollo-insurance-covertrack.yml\n- name: none declared\n  type: null\n  declared: false\n  applied: >-\n    The superseded affiliate generation declares an x-api-key header parameter on each operation\n    but no securitySchemes and no security requirement.\n  sources:\n  - openapi/apollo-insurance-affiliates-legacy.yml\n\nissuance:\n  self_serve: false\n  provisioning_ui: none\n  process: >-\n    Keys are issued\
  \ by hand by an APOLLO contact. The documentation is genuinely public — no\n    login wall, no gate, no sign-in prompt — but the integration is partner-scoped. Open docs,\n    closed credentials.\n  request_via: https://apollocover.com/partnerships\n  per_environment: true\n  environments:\n  - {mode: test, host: 'https://o73td82enk.execute-api.ca-central-1.amazonaws.com/1_0_0', api: Affiliates}\n  - {mode: live, host: 'https://fpl95knwc1.execute-api.ca-central-1.amazonaws.com/1_0_0', api: Affiliates}\n  - {mode: test, host: 'https://api.covertrack-dev.ca', api: CoverTrack}\n  - {mode: live, host: 'https://api.covertrack.ca', api: CoverTrack}\n  rotation: not published\n  expiry: not published\n  revocation: not published\n\nauthorization:\n  model: path-scoped\n  note: >-\n    The token carries no scopes, roles or claims. Every authorization boundary is a path\n    identifier the partner is given — affiliateId on the Affiliates API, and\n    partnerId/propertyId/tenantId on CoverTrack.\
  \ A key plus a guessed identifier is the only\n    thing between a caller and another partner's data, so identifier entropy is load-bearing.\n  scopes: none\n  detail: conventions/apollo-insurance-conventions.yml\n\nfailure_modes:\n  '403': Forbidden — invalid token, or a token from the other environment\n  '401': not documented on any operation\n  note: >-\n    APOLLO documents no 401 anywhere. An authentication failure surfaces as 403.\n\nend_user_auth:\n  present: false\n  note: >-\n    There is no consumer-facing API and no end-user authorization. Consumers authenticate only on\n    the hosted co-branded launchpad and in the customer portal\n    (https://policy-portal.apollocover.com/), neither of which has a documented API. APOLLO's\n    security page states end users can protect their APOLLO data with two-factor authentication\n    via email — that is a web-app control, not an API one.\n\ndiscovery:\n  well_known: none\n  openid_configuration: 404/403 on every host\n  oauth_authorization_server:\
  \ 404/403 on every host\n  detail: well-known/apollo-insurance-well-known.yml\n\ntransport_security:\n  tls_minimum_published: TLS v1.2 (per https://apollocover.com/security)\n  tls_observed: TLSv1.3 on apollocover.com, docs.apollocover.com, api.covertrack.ca and the API Gateway host\n  detail: security/apollo-insurance-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/authentication/apollo-insurance-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Insurance
- Canada
- Insurtech
- Broker
- Embedded Insurance
- Property and Casualty
- Tenant Insurance
- Quoting
- Distribution
- Compliance
---
