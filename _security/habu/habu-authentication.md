---
api_key_in: []
api_specs:
- filename: habu-clean-room-api-openapi.yml
  format: yaml
  label: Habu Clean Room API
  slug: habu-clean-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/openapi/habu-clean-room-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Habu Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Habu secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Habu
provider_slug: habu
scheme_count: 1
schemes:
- applied: 'globally, via the root security block (security: [{application: []}])'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.habu.com/v1/oauth/token
  name: application
  sources:
  - openapi/habu-clean-room-api-openapi.yml
  type: oauth2
slug: habu-authentication
source_filename: habu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.liveramp.com/clean-room-api/reference/request-an-access-token and https://developers.liveramp.com/clean-room-api/reference/configuring-a-clean-room-api-user,\n  reconciled against openapi/habu-clean-room-api-openapi.yml components.securitySchemes and live probes\n  of https://api.habu.com/v1/oauth/token (2026-08-12).\ndocs: https://developers.liveramp.com/clean-room-api/reference/request-an-access-token\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  scopes_defined: 0\n  model: OAuth 2.0 client-credentials service account. Authorization inside the API is by clean room ROLE,\n    not by OAuth scope — the flow declares an empty scopes object.\nschemes:\n- name: application\n  type: oauth2\n  applied: 'globally, via the root security block (security: [{application: []}])'\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.habu.com/v1/oauth/token\n    scopes: 0\n  sources:\n\
  \  - openapi/habu-clean-room-api-openapi.yml\nprovisioning:\n  where: A service account is created in the Clean Room console; client credentials are read from the\n    \"Manage API Key\" page.\n  docs: https://developers.liveramp.com/clean-room-api/reference/configuring-a-clean-room-api-user\n  note: Credentials cannot be created through the API. The docs state credential creation is deliberately\n    not exposed externally to avoid transmitting raw credential values.\ntoken_request:\n  method: POST\n  url: https://api.habu.com/v1/oauth/token\n  content_type: application/x-www-form-urlencoded\n  authorization_header: Basic base64(client_id:client_secret)\n  body: grant_type=client_credentials\n  response_fields:\n  - accessToken\n  - tokenType\n  - expiresIn\n  - expiresAt\n  token_type: Bearer\n  expires_in_seconds: 43200\n  issuance_limit: 2 tokens per 24-hour period per API user — reuse the token until it expires.\n  live_evidence:\n  - GET https://api.habu.com/v1/oauth/token → 405\
  \ {\"status\":\"METHOD_NOT_ALLOWED\",...} (POST only)\n  - 'POST with Content-Type: application/json → 415 {\"status\":\"UNSUPPORTED_MEDIA_TYPE\",\"message\":\"Content-Type\n    ''application/json'' is not supported\"}'\n  - POST form-encoded without an Authorization header → 400 {\"message\":\"Required request header 'Authorization'\n    for method parameter type String is not present\"}\ncall_authorization: 'Authorization: Bearer <accessToken> on every operation except GET /health, which\n  is unauthenticated.'\nunauthenticated_operations:\n- getHealth\ndiscovery:\n  openid_configuration: 404 on api.habu.com\n  oauth_authorization_server: 404 on api.habu.com\n  oauth_protected_resource: 404 on api.habu.com\n  note: No RFC 8414 / RFC 9728 discovery metadata is published; the token endpoint is only discoverable\n    from the OpenAPI and the docs.\ntransport:\n  tls: TLS 1.2 on api.habu.com\n  hsts: 'strict-transport-security: max-age=31536000 ; includeSubDomains'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habu/refs/heads/main/authentication/habu-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Data Clean Room
- Data Collaboration
- Advertising
- Privacy
- Identity
- Marketing
- Analytics
---
