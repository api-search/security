---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Amperity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Amperity secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Amperity
provider_slug: amperity
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    grant_type: client_credentials
    request_content_type: application/x-www-form-urlencoded
    request_params:
    - client_id
    - client_secret
    scopes: {}
    tokenUrl: https://{tenant}.amperity.com/api/v0/oauth2/token
    token_response:
      access_token: string
      expires_in: 3600
      token_type: Bearer
  name: OAuth2ClientCredentials
  sources:
  - https://docs.amperity.com/api/authentication.html
  type: oauth2
- applied_via: 'Authorization: Bearer ${access-token}'
  bearerFormat: JWT
  name: BearerJWT
  scheme: bearer
  sources:
  - https://docs.amperity.com/api/authentication.html
  type: http
slug: amperity-authentication
source_filename: amperity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.amperity.com/api/authentication.html\ndocs: https://docs.amperity.com/api/authentication.html\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials]\noverview: >-\n  Amperity APIs authenticate with a JWT bearer access token. An administrator creates an API key\n  (a synthetic identity bound to the tenant) under Settings > Security > API keys, granting it the\n  DataGrid Operator role. The API key's client_id/client_secret are exchanged for a short-lived\n  access token via the OAuth2 client-credentials token endpoint. All API requests then send the\n  token in the Authorization header, plus a tenant identifier header and a date-based api-version\n  header.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.amperity.com/api/v0/oauth2/token\n    grant_type: client_credentials\n\
  \    request_content_type: application/x-www-form-urlencoded\n    request_params: [client_id, client_secret]\n    token_response:\n      access_token: string\n      token_type: Bearer\n      expires_in: 3600\n    scopes: {}\n  sources: [https://docs.amperity.com/api/authentication.html]\n- name: BearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_via: 'Authorization: Bearer ${access-token}'\n  sources: [https://docs.amperity.com/api/authentication.html]\nrequired_headers:\n- name: Authorization\n  value: 'Bearer ${access-token}'\n  apis: [Amperity API, Profile API, Streaming API]\n- name: amperity-tenant\n  value: '{tenant-id}'\n  apis: [Profile API]\n- name: X-Amperity-Tenant\n  value: '{tenant-name}'\n  apis: [Amperity API, Streaming API]\n- name: api-version\n  value: 'YYYY-MM-DD (e.g. 2024-04-01 for Amperity API, 2025-07-31 for Profile API)'\n  apis: [Amperity API, Profile API]\ntoken_lifecycle:\n  format: JWT\n  expiry: 'expires_in seconds (default 3600); UI-generated\
  \ tokens expire after a configured number of days'\n  refresh: 'no refresh-grant flow; regenerate via client-credentials exchange or the UI'\n  key_rotation: 'rotating an API key mints a new secret; previously issued tokens remain valid for 30 days (deposed state) before becoming invalid'\nnotes:\n- API keys are managed under Settings > Security and require the API key administration policy.\n- The Streaming API uses a self-managed Streaming Ingest JWT token generated in the UI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amperity/refs/heads/main/authentication/amperity-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Enterprise
- Customer Data Platform
- CDP
- Identity Resolution
- Customer 360
- Marketing
- Data
- Profiles
- Analytics
---
