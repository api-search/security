---
api_key_in: []
auth_types:
- http
description: The Solarize API authenticates requests with short-lived JSON Web Tokens (JWT). A caller first mints a long-lived API Token inside the Solarize app (Settings), then exchanges it at the token endpoint for a Bearer access token. API Tokens carry the same permissions as the user that created them; there is no separate OAuth2 scope surface.
kind: authentication
layout: security
method: searched
name: Solarize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solarize secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Solarize
provider_slug: solarize
scheme_count: 2
schemes:
- detail: A long-lived API Token generated in the Solarize app. Exchanged (not sent directly on resource requests) at POST /v1/oauth for a JWT access token. Inherits the permissions of the generating user.
  name: apiToken
  type: prerequisite
- bearer_format: JWT
  detail: 'All resource requests send `Authorization: Bearer <accessToken>` over HTTPS. Plain-HTTP and unauthenticated requests fail. Access tokens expire (expiresIn ~3599s) and are renewed via the refresh token.'
  name: bearerAuth
  scheme: bearer
  type: http
slug: solarize-authentication
source_filename: solarize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api-docs.solarize.energy/authentication\ndocs: https://api-docs.solarize.energy/authentication\ndescription: >-\n  The Solarize API authenticates requests with short-lived JSON Web Tokens\n  (JWT). A caller first mints a long-lived API Token inside the Solarize app\n  (Settings), then exchanges it at the token endpoint for a Bearer access token.\n  API Tokens carry the same permissions as the user that created them; there is\n  no separate OAuth2 scope surface.\nsummary:\n  types: [http]\n  http_scheme: bearer\n  bearer_format: JWT\n  api_key_in: []\n  oauth2_flows: []\ntoken_endpoint:\n  url: https://api.solarize.energy/v1/oauth\n  method: POST\n  content_type: application/json\n  grant_type: api_token\n  request_example: '{\"grantType\":\"api_token\",\"token\":\"<API_TOKEN>\"}'\n  response_fields:\n    - accessToken\n    - refreshToken\n    - clientId\n    - tokenType   # Bearer\n    - expiresIn   # seconds, e.g.\
  \ 3599\n    - createdAt\nschemes:\n  - name: apiToken\n    type: prerequisite\n    detail: >-\n      A long-lived API Token generated in the Solarize app. Exchanged (not sent\n      directly on resource requests) at POST /v1/oauth for a JWT access token.\n      Inherits the permissions of the generating user.\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    detail: >-\n      All resource requests send `Authorization: Bearer <accessToken>` over\n      HTTPS. Plain-HTTP and unauthenticated requests fail. Access tokens expire\n      (expiresIn ~3599s) and are renewed via the refresh token.\nnotes:\n  - Calls made over plain HTTP fail; HTTPS is required.\n  - Access tokens are short-lived; use the returned refreshToken to obtain a new JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solarize/refs/heads/main/authentication/solarize-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Energy
- Billing
- Metering
- Utilities
- Meter-to-Cash
- SaaS
---
