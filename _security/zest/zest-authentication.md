---
api_key_in: []
api_specs:
- filename: zest-openapi-original.json
  format: json
  label: Zest Public API
  slug: zest-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zest/refs/heads/main/openapi/zest-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zest secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zest
provider_slug: zest
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/zest-openapi-original.json
  type: http
slug: zest-authentication
source_filename: zest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zest-openapi-original.json\ndocs: https://docs.zestequity.com/api-reference/authentication/exchange-a-jwt-assertion-for-an-access-token\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_grants:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\nmodel: >-\n  Partner-signed JWT-Bearer assertion grant (RFC 7523). The partner mints a\n  short-lived JWT signed with an EdDSA private key registered with Zest, then\n  exchanges it at POST /v1/oauth2/tokens for a short-lived bearer access token.\n  The bearer token is sent in the Authorization header on every partner API\n  call. HTTPBearer is the only OpenAPI-declared security scheme.\njwt_assertion_claims:\n  iss: Partner API base URL\n  sub: Partner client_id\n  aud: https://sandbox-api.zestequity.com\n  client_id: Partner client_id\n  iat: now (unix seconds)\n  exp: now + 60\nsigning_algorithm: EdDSA\ntoken_endpoint: https://sandbox-api.zestequity.com/v1/oauth2/tokens\n\
  token_response:\n  accessToken: bearer JWT\n  refreshToken: JWT\n  tokenType: Bearer\n  expiresIn: 3600\n  refreshExpiresIn: 2592000\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zest-openapi-original.json\nprovisioning: >-\n  Sandbox client_id, the matching EdDSA private key, and a registered webhook\n  URL + signing secret are provisioned during partner onboarding. Contact\n  sara@zestholdco.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zest/refs/heads/main/authentication/zest-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- SPV
- Private Markets
- Fintech
- Equity
- Investors
- Escrow
- SPaaS
- MENA
- API
---
