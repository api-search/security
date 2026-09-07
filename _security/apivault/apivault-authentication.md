---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apivault-api-openapi.yml
  format: yaml
  label: Apivault
  slug: apivault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apivault/refs/heads/main/openapi/apivault-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apivault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apivault secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apivault
provider_slug: apivault
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'SimpleJWT bearer token, sent as `Authorization: Bearer <jwt>`.'
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/_original/apivault-openapi.yml
  type: http
slug: apivault-authentication
source_filename: apivault-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/_original/apivault-openapi.yml (harvested from\n  https://api.apivault.dev/api/schema/) upgraded from the provider's own source\n  (backend/authentication/urls.py, backend/apivault/settings.py and\n  frontend/services/ApivaultServices.ts in\n  https://github.com/exa-studio/ApiVault) and from live 401/406 probes of\n  https://api.apivault.dev on 2026-09-04.\ndocs: https://api.apivault.dev/api/schema/swagger-ui/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_access: true\n  human_identity_required: true\nschemes:\n  - name: jwtAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources: [openapi/_original/apivault-openapi.yml]\n    description: >-\n      SimpleJWT bearer token, sent as `Authorization: Bearer <jwt>`.\ntoken_acquisition:\n  method: google-sign-in-exchange\n  note: >-\n    There is NO API key, no client-credentials\
  \ grant and no self-service\n    developer key. The only way to obtain a token is to sign in to\n    apivault.dev with a Google account in a browser and exchange the resulting\n    Google token: POST /api/auth/google/ (operationId auth_google_create) with\n    an `auth_token` body field returns the SimpleJWT access/refresh pair.\n    This is the single largest agent-readiness constraint on this API — an\n    unattended agent cannot mint credentials.\n  operations:\n    - {operationId: auth_google_create, path: /api/auth/google/, method: POST}\n    - {operationId: auth_token_refresh_create, path: /api/auth/token/refresh/, method: POST}\n    - {operationId: auth_token_verify_create, path: /api/auth/token/verify/, method: POST}\n    - {operationId: auth_user_retrieve, path: /api/auth/user/, method: GET}\nanonymous_surface:\n  note: >-\n    Nine of the eighteen operations declare `security: [{jwtAuth: []}, {}]`,\n    the OpenAPI form for \"token optional\". All nine were confirmed to answer\n\
  \    200 with no credentials on 2026-09-04.\n  verified_anonymous:\n    - {operationId: all_list, path: /api/all, status: 200}\n    - {operationId: categories_list, path: /api/categories, status: 200}\n    - {operationId: categories_trending_list, path: /api/categories/trending, status: 200}\n    - {operationId: count_retrieve, path: /api/count, status: 200}\n    - {operationId: random_list, path: /api/random, status: 200}\n    - {operationId: search_list, path: /api/search, status: 200}\nauthenticated_only:\n  - {operationId: auth_user_retrieve, observed_status_without_token: 401}\n  - {operationId: my_api_retrieve, observed_status_without_token: 401}\n  - {operationId: pending_my_api_retrieve, observed_status_without_token: 401}\n  - {operationId: create_create, observed_status_without_token: 401}\n  - {operationId: interaction_like_create, observed_status_without_token: 401}\n  - {operationId: interaction_like_destroy, observed_status_without_token: 401}\n  - {operationId: interaction_feedback_create,\
  \ observed_status_without_token: 401}\nchallenge:\n  status: 401\n  body: '{\"detail\": \"Authentication credentials were not provided.\"}'\n  www_authenticate: not sent\n  note: >-\n    The 401 carries no WWW-Authenticate header, so a client cannot discover the\n    scheme from the challenge — it has to read the spec.\nscopes: none\ngaps:\n  - No WWW-Authenticate challenge header on 401.\n  - No token lifetime, rotation or revocation policy is published.\n  - No machine-to-machine credential of any kind; Google sign-in is mandatory.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apivault/refs/heads/main/authentication/apivault-authentication.yml
summary_line: http · 1 scheme
tags:
- API Catalog
- API Directory
- API Discovery
- Open-Source
- Public APIs
---
