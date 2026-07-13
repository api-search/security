---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Zeplin API
  slug: zeplin-api
  spec_type: OpenAPI
  url: https://github.com/zeplin/openapi
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zeplin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zeplin secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zeplin
provider_slug: zeplin
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /v1/oauth/token
  name: OAuth2
  sources:
  - openapi/zeplin-zeplin-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - openapi/zeplin-zeplin-api-openapi.yml
  type: http
slug: zeplin-authentication
source_filename: zeplin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeplin-zeplin-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/zeplin-zeplin-api-openapi.yml\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zeplin-zeplin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/authentication/zeplin-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhooks
---
