---
api_key_in: []
api_specs:
- filename: cintoo-openapi-original.json
  format: json
  label: Cintoo Open API
  slug: cintoo-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/openapi/cintoo-openapi-original.json
auth_types:
- oauth2
- http-bearer-jwt
description: ''
kind: authentication
layout: security
method: searched
name: Cintoo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cintoo secures its APIs with oauth2 and http-bearer-jwt across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cintoo
provider_slug: cintoo
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://aec.cintoo.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://aec.cintoo.com/oauth/token
    scopes: 0
    tokenUrl: https://aec.cintoo.com/oauth/token
  name: oauth2
  sources:
  - openapi/cintoo-openapi-original.json
  type: oauth2
slug: cintoo-authentication
source_filename: cintoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://aec.cintoo.com/api/2 (Authentication section) + openapi/cintoo-openapi-original.json\ndocs: https://aec.cintoo.com/api/2\nsummary:\n  types:\n  - oauth2\n  - http-bearer-jwt\n  oauth2_flows:\n  - authorizationCode\n  token_format: JWT\nmodel: >-\n  The Cintoo API relies on JWT tokens with the standard Access Token + Refresh Token pair.\n  The first acquisition of the token pair requires a manual step (via the cintoo-login CLI or\n  OAuth authorize flow) for security reasons; afterward it can be fully automated. Every request\n  (except the authentication endpoints) carries `Authorization: Bearer <access_token>`.\ntokens:\n  access_token:\n    ttl: 3h\n    stateless: true\n    usage: authenticates each API call; may be used in parallel (no concurrent limit)\n  refresh_token:\n    ttl: months\n    stateful: true\n    single_use: true\n    concurrent_limit: 10 valid refresh tokens per user\n    usage: used once to obtain\
  \ a new Access Token + Refresh Token pair; cannot make API calls\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://aec.cintoo.com/oauth/authorize\n    tokenUrl: https://aec.cintoo.com/oauth/token\n    refreshUrl: https://aec.cintoo.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/cintoo-openapi-original.json\nbootstrap:\n  cli: cintoo-login-1.1.0-signed.exe\n  see: cli/cintoo-cli.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cintoo/refs/heads/main/authentication/cintoo-authentication.yml
summary_line: oauth2/http-bearer-jwt · 1 scheme
tags:
- Company
- Infrastructure SaaS
- Reality Capture
- Digital Twin
- Point Cloud
- 3D
- AEC
- BIM
- Construction
- Scan-to-BIM
- GIS
---
