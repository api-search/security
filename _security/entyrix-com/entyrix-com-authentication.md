---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Entyrix Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: entyrix-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: entyrix-com
provider_slug: entyrix-com
scheme_count: 2
schemes:
- authorizationUrl: /oauth/authorize
  flow: authorization_code
  pkce: true
  scopes:
  - mcp:read
  - fo:read
  - api:read
  tokenUrl: /oauth/token
  type: oauth2
- description: Bearer sk_<token>
  in: header
  name: Authorization
  type: apiKey
slug: entyrix-com-authentication
source_filename: entyrix-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://entyrix.com/llms.txt\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    pkce: true\n    tokenUrl: \"/oauth/token\"\n    authorizationUrl: \"/oauth/authorize\"\n    scopes:\n      - \"mcp:read\"\n      - \"fo:read\"\n      - \"api:read\"\n  - type: apiKey\n    name: \"Authorization\"\n    in: \"header\"\n    description: \"Bearer sk_<token>\"\n"
source_yaml_url: https://artifacts.apis.io/entyrix-com/authentication/entyrix-com-authentication.yml
summary_line: 2 schemes
tags:
- BusinessData
- Compliance
- KYC
- API
- European
---
