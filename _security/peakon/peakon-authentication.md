---
api_key_in: []
api_specs:
- filename: peakon-actions-api-openapi.yml
  format: yaml
  label: Peakon Actions API
  slug: peakon-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-actions-api-openapi.yml
- filename: peakon-answers-api-openapi.yml
  format: yaml
  label: Peakon Answers API
  slug: peakon-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-answers-api-openapi.yml
- filename: peakon-audits-api-openapi.yml
  format: yaml
  label: Peakon Audits API
  slug: peakon-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-audits-api-openapi.yml
- filename: peakon-authentication-api-openapi.yml
  format: yaml
  label: Peakon Authentication API
  slug: peakon-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-authentication-api-openapi.yml
- filename: peakon-employees-api-openapi.yml
  format: yaml
  label: Peakon Employees API
  slug: peakon-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-employees-api-openapi.yml
- filename: peakon-engagement-api-openapi.yml
  format: yaml
  label: Peakon Engagement API
  slug: peakon-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-engagement-api-openapi.yml
- filename: peakon-scores-api-openapi.yml
  format: yaml
  label: Peakon Scores API
  slug: peakon-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-scores-api-openapi.yml
- filename: peakon-segments-api-openapi.yml
  format: yaml
  label: Peakon Segments API
  slug: peakon-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/openapi/peakon-segments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Peakon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peakon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Peakon
provider_slug: peakon
scheme_count: 1
schemes:
- applied_to: all operations except POST /auth/application
  bearer_format: JWT
  description: Session bearer token returned by POST /auth/application as a JSON:API resource of type `bearer_tokens`. Applied to every operation except the auth exchange itself.
  name: jwt
  scheme: bearer
  sources:
  - openapi/peakon-openapi-original.json
  type: http
slug: peakon-authentication
source_filename: peakon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.peakon.com/docs/getting-started\ndocs: https://developer.peakon.com/docs/getting-started\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\nmodel: >-\n  Two-step application authentication. A developer creates a Custom App in the Peakon\n  dashboard (Integrations > Custom Apps), selecting a set of permissions that scope the\n  app to specific areas of the API. Creating the app yields a long-lived application\n  access token (shown once, treated as a secret). The application exchanges that token\n  for a short-lived session token (JWT) by POSTing it to /auth/application; the JWT is\n  then sent as `Authorization: Bearer <jwt>` on all subsequent API calls. Passing\n  `persists: true` on the exchange returns a session that never expires.\nschemes:\n  - name: jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      Session\
  \ bearer token returned by POST /auth/application as a JSON:API resource of\n      type `bearer_tokens`. Applied to every operation except the auth exchange itself.\n    applied_to: all operations except POST /auth/application\n    sources: [openapi/peakon-openapi-original.json]\ntoken_exchange:\n  operation: POST /auth/application\n  request: { token: <application access token>, persists: <bool> }\n  response: JSON:API resource of type bearer_tokens (id = the JWT)\npermissions:\n  model: per-application permission areas selected at app-creation time\n  guidance: >-\n    Grant as few permissions as possible; each permission grants access to one area of\n    the API. Peakon does not expose an OAuth2 scope endpoint - permissions are chosen in\n    the dashboard, not requested via an OAuth flow.\nscim:\n  note: >-\n    A separate SCIM 2.0 provisioning API (base https://{subdomain}.peakon.com/api/scim/v2)\n    also uses Bearer token authentication, with a token obtained from the Employee\n\
  \    Provisioning integration.\n  docs: https://developer.peakon.com/docs/building-a-scim-20-api-connector\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peakon/refs/heads/main/authentication/peakon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Employee Engagement
- Employee Experience
- HR Tech
- Surveys
- People Analytics
- Workday
---
