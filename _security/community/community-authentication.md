---
api_key_in: []
api_specs:
- filename: community-async-openapi-original.yml
  format: yaml
  label: Community Async REST API
  slug: community-async-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-async-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Community Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Community secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Community
provider_slug: community
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/community-async-openapi-original.yml
  type: http
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    scopes: 0
    tokenUrl: /oauth/v1/token
  name: oAuth
  sources:
  - openapi/community-async-openapi-original.yml
  type: oauth2
slug: community-authentication
source_filename: community-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/community-async-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/community-async-openapi-original.yml\n- name: oAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: /oauth/v1/token\n    scopes: 0\n  sources:\n  - openapi/community-async-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/authentication/community-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Messaging
- SMS
- Communications
- Conversational
- Marketing
- Creators
- Webhooks
- Company
---
