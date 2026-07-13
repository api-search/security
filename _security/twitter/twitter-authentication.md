---
api_key_in: []
api_specs:
- filename: x-api-openapi.json
  format: json
  label: X API
  slug: x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/x-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Twitter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: X (Twitter) secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: X (Twitter)
provider_slug: twitter
scheme_count: 3
schemes:
- name: BearerToken
  scheme: bearer
  sources:
  - openapi/x-api-openapi.json
  type: http
- flows:
  - authorizationUrl: https://api.x.com/2/oauth2/authorize
    flow: authorizationCode
    scopes: 21
    tokenUrl: https://api.x.com/2/oauth2/token
  name: OAuth2UserToken
  sources:
  - openapi/x-api-openapi.json
  type: oauth2
- name: UserToken
  scheme: OAuth
  sources:
  - openapi/x-api-openapi.json
  type: http
slug: twitter-authentication
source_filename: twitter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/x-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/x-api-openapi.json\n- name: OAuth2UserToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.x.com/2/oauth2/authorize\n    tokenUrl: https://api.x.com/2/oauth2/token\n    scopes: 21\n  sources:\n  - openapi/x-api-openapi.json\n- name: UserToken\n  type: http\n  scheme: OAuth\n  sources:\n  - openapi/x-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/authentication/twitter-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
---
