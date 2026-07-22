---
api_key_in:
- body
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Verbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: VerbIT secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VerbIT
provider_slug: verbit
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Short-lived JSON Web Token (JWT) passed in the Authorization header as "Authorization: bearer <token>". The token is minted by POSTing the customer api_key to the Verbit auth service and expires 24 hours after creation.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://verbit.readme.io/docs/authentication
  token_endpoint: https://users.verbit.co/api/v1/auth
  token_request: 'POST {"data": {"api_key": "<API-KEY>"}}'
  token_response_field: token
  token_ttl_seconds: 86400
  type: http
- description: Legacy per-request API token supported for existing post-production API integrations. Still valid, but new integrations should use the JWT bearer flow. Post-production APIs may also use the JWT scheme.
  in: query
  name: api_token
  sources:
  - https://verbit.readme.io/docs/api-token
  type: apiKey
slug: verbit-authentication
source_filename: verbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://verbit.readme.io/docs/authentication\ndocs: https://verbit.readme.io/docs/authentication\nsummary:\n  types: [http, apiKey]\n  http_scheme: bearer\n  bearer_format: JWT\n  api_key_in: [body]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived JSON Web Token (JWT) passed in the Authorization header as\n      \"Authorization: bearer <token>\". The token is minted by POSTing the\n      customer api_key to the Verbit auth service and expires 24 hours after\n      creation.\n    token_endpoint: https://users.verbit.co/api/v1/auth\n    token_request: 'POST {\"data\": {\"api_key\": \"<API-KEY>\"}}'\n    token_response_field: token\n    token_ttl_seconds: 86400\n    sources: [https://verbit.readme.io/docs/authentication]\n  - name: legacyApiToken\n    type: apiKey\n    in: query\n    name: api_token\n    description: >-\n    \
  \  Legacy per-request API token supported for existing post-production API\n      integrations. Still valid, but new integrations should use the JWT bearer\n      flow. Post-production APIs may also use the JWT scheme.\n    sources: [https://verbit.readme.io/docs/api-token]\nnotes: >-\n  API key generation requires the Admin role on the Verbit platform. A separate\n  order-level / permanent customer token is used for the streaming WebSocket\n  endpoint (wss://speech.verbit.co/ws). No OAuth2 authorization/token scope\n  surface is documented (access is governed by platform RBAC roles such as\n  customer_admin / customer_content_manager), so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verbit/refs/heads/main/authentication/verbit-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Ai Enterprise Software
- Transcription
- Captioning
- Speech Recognition
- Accessibility
- Artificial Intelligence
- Media
---
