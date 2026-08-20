---
api_key_in:
- header
api_specs:
- filename: later-influence-api-openapi.json
  format: json
  label: Later Influence API
  slug: later-influence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/later/refs/heads/main/openapi/later-influence-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Later Authentication
name_suffix: Authentication
oauth_flows: []
overview: Later secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Later
provider_slug: later
scheme_count: 2
schemes:
- applies_to: brand/admin operations (the default `security` block of the contract)
  declared: true
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/later-influence-api-openapi.json
  type: apiKey
- applies_to: influencer-facing operations under /v1/later-influencers/{influencerIdOrCreatorId} and the Authentication tag token-exchange operations
  bearer_format: JWT
  declared: false
  evidence:
  - detail: '"Pass an email and password in exchange for a JWT to include in the header of requests." — POST /email-auth/login (Authentication tag)'
    kind: operation-description
    source: openapi/later-influence-api-openapi.json
  - body: '{"message":"Unauthorized - Unable to verify the signed JWT token."}'
    fetched: '2026-08-13'
    http_status: 401
    kind: live-probe
    url: https://api.mavrck.co/v1/later-influencers/1
  name: jwt
  scheme: bearer
  sources:
  - openapi/later-influence-api-openapi.json
  type: http
slug: later-authentication
source_filename: later-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/later-influence-api-openapi.json\nnote: >-\n  Derived from the Later Influence (formerly Mavrck) Swagger 2.0 contract published at\n  https://api.mavrck.co/api-docs, then confirmed against live unauthenticated probes of\n  https://api.mavrck.co/v1/*. The contract declares ONE security definition (an `api-key`\n  header) but the operation descriptions and the live 401 bodies show a SECOND, distinct\n  credential in use on the influencer-facing surface: a JWT minted by the /email-auth,\n  /api-key/facebook and /auto-login operations and sent on subsequent requests. Later\n  publishes no public developer portal for either surface, so no docs URL upgrades this\n  to method searched.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  declared: true\n  applies_to:\
  \ brand/admin operations (the default `security` block of the contract)\n  sources:\n  - openapi/later-influence-api-openapi.json\n- name: jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  declared: false\n  applies_to: >-\n    influencer-facing operations under /v1/later-influencers/{influencerIdOrCreatorId}\n    and the Authentication tag token-exchange operations\n  evidence:\n  - kind: operation-description\n    detail: >-\n      \"Pass an email and password in exchange for a JWT to include in the header of\n      requests.\" — POST /email-auth/login (Authentication tag)\n    source: openapi/later-influence-api-openapi.json\n  - kind: live-probe\n    url: https://api.mavrck.co/v1/later-influencers/1\n    http_status: 401\n    body: '{\"message\":\"Unauthorized - Unable to verify the signed JWT token.\"}'\n    fetched: '2026-08-13'\n  sources:\n  - openapi/later-influence-api-openapi.json\ntoken_exchange_operations:\n- method: POST\n  path: /email-auth/login\n  summary: Pass\
  \ an email and password in exchange for a JWT.\n- method: POST\n  path: /email-auth/signup\n  summary: Pass an email verification request key and new password in exchange for a JWT.\n- method: POST\n  path: /email-auth/reset-password\n  summary: Pass an email reset password request key and new password in exchange for a JWT.\n- method: POST\n  path: /api-key/facebook\n  summary: Pass Facebook access grant information in exchange for a JWT.\n- method: POST\n  path: /connected-account/instagram-business\n  summary: Pass Facebook access grant information in exchange for a JWT.\n- method: POST\n  path: /auto-login\n  summary: Pass an encrypted user key in exchange for a JWT.\n- method: POST\n  path: /v1/api-key/login\n  operationId: loginAdmin\n- method: POST\n  path: /v1/api-key/swap-app\n  operationId: swapCommunity\n- method: POST\n  path: /v1/auth/facebook/exchange-code-for-token\n  operationId: exchangeCodeForToken\nunauthenticated_behavior:\n- url: https://api.mavrck.co/v1/influencers\n\
  \  http_status: 403\n  body: '{\"type\":\"RESOURCE_FORBIDDEN_ERROR\",\"error\":\"Access to this resource is forbidden.\"}'\n  fetched: '2026-08-13'\n- url: https://api.mavrck.co/v1/action-groups\n  http_status: 403\n  body: '{\"type\":\"RESOURCE_FORBIDDEN_ERROR\",\"error\":\"Access to this resource is forbidden.\"}'\n  fetched: '2026-08-13'\ngaps:\n- The contract declares no oauth2, openIdConnect or mutualTLS scheme, so no OAuth scope\n  reference can be derived; scopes/ is intentionally absent.\n- The JWT credential is used but undeclared in `securityDefinitions`, so a generated\n  client will not send it.\n- No public credential-provisioning documentation is published on later.com; api-key\n  issuance appears to be account-managed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/later/refs/heads/main/authentication/later-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Social-Media
- Scheduling
- Instagram
- TikTok
- Influencer Marketing
- Content Management
- Analytics
- Social Commerce
---
