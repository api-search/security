---
api_key_in:
- header
api_specs:
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Engagements API
  slug: chorus-engagements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus Recordings & Transcripts API
  slug: chorus-recordings-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
- filename: chorus-ai-openapi.yml
  format: yaml
  label: Chorus CRM Sync API
  slug: chorus-crm-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/openapi/chorus-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Chorus Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chorus.ai secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chorus.ai
provider_slug: chorus-ai
scheme_count: 3
schemes:
- applies_to: subset of operations; the spec does not enumerate which
  description: HTTP basic authentication (for those APIs that support it).
  name: basic
  scheme: basic
  sources:
  - openapi/chorus-ai-openapi.yml
  type: http
- description: A Chorus token or a signed JWT.
  name: bearer-token
  scheme: bearer
  sources:
  - openapi/chorus-ai-openapi.yml
  type: http
- description: A ZoomInfo access token.
  in: header
  name: x-ziaccesstoken
  note: Post-acquisition path — a ZoomInfo-issued access token is accepted as an alternative to a native Chorus API token. Chorus.ai was acquired by ZoomInfo in 2021 and now ships as "Chorus by ZoomInfo".
  parameter: x-ziaccesstoken
  sources:
  - openapi/chorus-ai-openapi.yml
  type: apiKey
slug: chorus-ai-authentication
source_filename: chorus-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://chorus.ai/api/openapi.json (info.description) + https://chorus.ai/api-docs/index.html\ndocs: https://chorus.ai/api-docs/index.html\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  primary: api_token_authorization_header\n  oauth2: false\n  notes: >-\n    The Chorus API authenticates with a per-user API token sent in the Authorization header.\n    Note the divergence between the published spec and the published prose: the OpenAPI declares\n    an http/bearer scheme, but info.description demonstrates a RAW token with no \"Bearer \" prefix\n    (curl -H \"Authorization:<token>\"). Clients written from the spec alone may send the wrong shape.\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: HTTP basic authentication (for those APIs that support it).\n  applies_to: subset of operations; the spec does not enumerate which\n  sources:\n  - openapi/chorus-ai-openapi.yml\n- name:\
  \ bearer-token\n  type: http\n  scheme: bearer\n  description: A Chorus token or a signed JWT.\n  sources:\n  - openapi/chorus-ai-openapi.yml\n- name: x-ziaccesstoken\n  type: apiKey\n  in: header\n  parameter: x-ziaccesstoken\n  description: A ZoomInfo access token.\n  note: >-\n    Post-acquisition path — a ZoomInfo-issued access token is accepted as an alternative to a\n    native Chorus API token. Chorus.ai was acquired by ZoomInfo in 2021 and now ships as\n    \"Chorus by ZoomInfo\".\n  sources:\n  - openapi/chorus-ai-openapi.yml\napplied:\n  global_security:\n  - basic\n  - bearer-token\n  - x-ziaccesstoken\n  note: All three schemes are declared at the document root as alternatives (OR).\ntoken_lifecycle:\n  issuance: >-\n    API tokens are generated per Chorus user from the Personal Settings page inside the Chorus\n    application. The user's role must be permitted API access via roles & permissions settings.\n  self_serve: false\n  gate: >-\n    The published docs state that during\
  \ the early access period a personal API token must be\n    obtained by contacting your Chorus customer success manager.\n  rotation: not documented\n  expiry: not documented\nauthorization_model:\n  style: user-scoped, inherits application permissions\n  rules:\n  - Recordings marked private are never returned through the API.\n  - >-\n    Data access control settings configured for the token's user apply to API access — to read all\n    recordings the token's user must themselves have access to all recordings.\n  - Roles & permissions that gate actions in the Chorus UI equally gate them through the API.\n  source: https://chorus.ai/api/openapi.json (info.description, \"Privacy and Data Access Control\")\nsession_endpoints:\n  note: >-\n    The spec also exposes interactive session management (POST /login, GET|DELETE\n    /api/v1/sessions/current, POST /api/v1/sessions/exchange, POST /api/auth/signed_request).\n    These back the Chorus web application rather than server-to-server API\
  \ token use.\n  operations:\n  - post-login\n  - get-api-v1-sessions-current\n  - delete-api-v1-sessions-current\n  - post-api-v1-sessions-exchange\n  - post-api-auth-signed_request\nscopes:\n  published: false\n  note: >-\n    No oauth2 securityScheme is declared and no scope reference is published, so there is no\n    scopes/ artifact for this provider. Authorization is role-based inside the Chorus product.\ncross_links:\n  conventions: conventions/chorus-ai-conventions.yml\n  errors: errors/chorus-ai-problem-types.yml\n  conformance: conformance/chorus-ai-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chorus-ai/refs/heads/main/authentication/chorus-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- ZoomInfo
- Conversation Intelligence
- Sales Enablement
- Call Recording
- Transcription
- Speech Analytics
- CRM
- Coaching
---
