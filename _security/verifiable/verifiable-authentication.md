---
api_key_in: []
api_specs:
- filename: verifiable-openapi-original.json
  format: json
  label: Verifiable API
  slug: verifiable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verifiable/refs/heads/main/openapi/verifiable-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Verifiable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verifiable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Verifiable
provider_slug: verifiable
scheme_count: 1
schemes:
- bearerFormat: custom
  description: 'Enter your bearer token in the format: Bearer {your token}'
  header: Authorization
  name: Bearer
  scheme: bearer
  sources:
  - openapi/verifiable-openapi-deprecated.json
  - openapi/verifiable-openapi-original.json
  type: http
slug: verifiable-authentication
source_filename: verifiable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/verifiable-openapi-original.json\ndocs: https://docs.discovery.verifiable.com/references/api/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_exchange_flows:\n  - password\n  - google-signin\n  - oauth-client-credentials\n  - sso\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: custom\n  header: Authorization\n  description: 'Enter your bearer token in the format: Bearer {your token}'\n  sources:\n  - openapi/verifiable-openapi-deprecated.json\n  - openapi/verifiable-openapi-original.json\ntoken_endpoints:\n- flow: password\n  operation: PasswordAuth\n  path: POST /auth/token/password\n  description: Exchange a registered email + password for an access token.\n- flow: google-signin\n  operation: GoogleAuth\n  path: POST /auth/token/google\n  description: Server-side Google Sign-In flow; exchange a Google auth code for an access token.\n- flow: oauth-client-credentials\n\
  \  operation: OAuthToken\n  path: POST /auth/oauth/token\n  premium: true\n  description: >-\n    Machine-to-machine OAuth 2.0 client credentials flow (client_id +\n    client_secret, grant_type=client_credentials). Premium add-on that must be\n    enabled per organization by the Verifiable team. No scopes are documented.\n- flow: sso\n  operation: SsoAuth\n  path: POST /auth/token/oauth\n  description: SSO-based authentication (premium/provisioned).\ntoken_management:\n- operation: ListActiveAccessTokens\n  path: GET /auth/token\n- operation: InvalidateAccessToken\n  path: POST /auth/token/{tokenId}/invalidate\n- operation: InvalidateAccessTokens\n  path: POST /auth/token/invalidate\nnotes: >-\n  No official first-party SDK is published; Verifiable recommends generating a\n  client from the OpenAPI description or using any HTTP client. There is no\n  OAuth scope surface, so scopes/ is intentionally omitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verifiable/refs/heads/main/authentication/verifiable-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- Credentialing
- Provider Data
- Primary Source Verification
- Compliance
- Monitoring
- API
---
