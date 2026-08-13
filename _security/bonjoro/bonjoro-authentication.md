---
api_key_in: []
api_specs:
- filename: bonjoro-api-v2-openapi.yml
  format: yaml
  label: Bonjoro API V2
  slug: bonjoro-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonjoro/refs/heads/main/openapi/bonjoro-api-v2-openapi.yml
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: derived
name: Bonjoro Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
- authorizationCode
overview: Bonjoro secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, clientCredentials, and authorizationCode flow(s).
provider_name: Bonjoro
provider_slug: bonjoro
scheme_count: 2
schemes:
- declared_in_spec: false
  grant_type_source: components.schemas.authenticationPayload.grant_type enum
  grant_types:
  - password
  - client_credentials
  - authorization_code
  name: OAuth
  operation: authenticate
  referenced_by_operations: 116
  request_fields:
  - grant_type
  - username
  - password
  - client_id
  - client_secret
  sources:
  - openapi/bonjoro-api-v2-openapi.yml
  token_response:
    expires_in_example: 31536000
    format: JWT (per spec example prefix eyJ0eXAiOiJKV1QiLCJh...)
    refresh_token: true
    token_type: Bearer
  token_url: https://www.bonjoro.com/api/v2/oauth/2/token
  type: oauth2
- declared_in_spec: false
  name: bearer
  scheme: bearer
  sources:
  - probe https://www.bonjoro.com/api/v2/greets
  type: http
  usage: 'Authorization: Bearer <access_token> against https://www.bonjoro.com/api/v2. Confirmed live: an unauthenticated GET of /api/v2/greets returns HTTP 401 with {"message":"Unauthenticated."}-shaped JSON, while the two open operations (/api/v2/industries, /api/v2/pricing) require no credential.'
slug: bonjoro-authentication
source_filename: bonjoro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/_original/bonjoro-api-v2-openapi-original.json\ndocs: https://vimily.github.io/bonjoro-api-docs/\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  api_key_in: []\n  oauth2_flows:\n  - password\n  - clientCredentials\n  - authorizationCode\nnotes: >-\n  The published Bonjoro API V2 definition declares NO `components.securitySchemes` block, yet 116 of its\n  123 operations carry `security: [{ OAuth: [] }]`. The `OAuth` scheme name is therefore an unresolved\n  reference — a real defect in the contract, not an absence of authentication. The auth model below is\n  derived from the token operation (`authenticate`, POST /api/v2/oauth/2/token), its request/response\n  schemas, and the `Bearer` token_type the spec's own example returns.\nschemes:\n- name: OAuth\n  type: oauth2\n  declared_in_spec: false\n  referenced_by_operations: 116\n  token_url: https://www.bonjoro.com/api/v2/oauth/2/token\n  operation: authenticate\n\
  \  grant_types:\n  - password\n  - client_credentials\n  - authorization_code\n  grant_type_source: components.schemas.authenticationPayload.grant_type enum\n  request_fields:\n  - grant_type\n  - username\n  - password\n  - client_id\n  - client_secret\n  token_response:\n    token_type: Bearer\n    expires_in_example: 31536000\n    refresh_token: true\n    format: JWT (per spec example prefix eyJ0eXAiOiJKV1QiLCJh...)\n  sources:\n  - openapi/bonjoro-api-v2-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  declared_in_spec: false\n  usage: >-\n    Authorization: Bearer <access_token> against https://www.bonjoro.com/api/v2. Confirmed live: an\n    unauthenticated GET of /api/v2/greets returns HTTP 401 with {\"message\":\"Unauthenticated.\"}-shaped\n    JSON, while the two open operations (/api/v2/industries, /api/v2/pricing) require no credential.\n  sources:\n  - probe https://www.bonjoro.com/api/v2/greets\nscopes:\n  declared: 0\n  note: >-\n    Every operation-level requirement\
  \ is `OAuth: []` — an empty scope array. Bonjoro publishes no OAuth\n    scope vocabulary, so no scopes/ artifact is emitted.\nunauthenticated_operations:\n- getIndustries\n- getPricing\n- loginViaGoogle\n- loginViaBranch\n- addUser\n- authenticate\nkey_management:\n  console: https://www.bonjoro.com/settings/api\n  note: >-\n    API credentials are issued from the in-app settings screen (login required). The Bonjoro help centre\n    documents key issuance at help.bonjoro.com; that host answers HTTP 403 to non-browser clients behind\n    a Cloudflare interactive challenge, so it could not be captured verbatim.\nx-evidence:\n- url: https://www.bonjoro.com/api/v2/greets\n  http_status: 401\n  fetched: '2026-08-12'\n- url: https://www.bonjoro.com/api/v2/industries\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://vimily.github.io/bonjoro-api-docs/\n  http_status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonjoro/refs/heads/main/authentication/bonjoro-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- video-messaging
- customer-engagement
- customer-success
- sales-engagement
- marketing-automation
- video
- crm-integration
- testimonials
- saas
- australia
---
