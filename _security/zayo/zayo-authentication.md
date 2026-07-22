---
api_key_in: []
api_specs:
- filename: zayo-openapi-original.yml
  format: yaml
  label: Zayo APIs
  slug: zayo-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zayo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zayo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zayo
provider_slug: zayo
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token authentication.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/zayo-openapi-original.yml
  type: http
- description: OAuth 2.0 using the Client Credentials grant type.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.api.zayo.com/oauth/token
  name: OAuthClientCredentials
  sources:
  - openapi/zayo-openapi-original.yml
  type: oauth2
slug: zayo-authentication
source_filename: zayo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/zayo-openapi-original.yml\ndocs: https://developer.zayo.com/docs/getting-started\ntoken_ttl_seconds: 3600\ntoken_type: Bearer\nnotes: >-\n  OAuth 2.0 Client Credentials grant; POST client_id/client_secret + grant_type=client_credentials\n  + scope=openid to https://auth.api.zayo.com/oauth/token. Bearer token valid 1 hour; re-request on 401.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication.\n  sources:\n  - openapi/zayo-openapi-original.yml\n- name: OAuthClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.zayo.com/oauth/token\n    scopes: 1\n  description: OAuth 2.0 using the Client Credentials grant type.\n  sources:\n  - openapi/zayo-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/authentication/zayo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Telecommunications
- Networking
- Connectivity
- Fiber
- Infrastructure
- Bandwidth
- Cloud Connectivity
- Ordering
- Ticketing
---
