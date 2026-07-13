---
api_key_in: []
api_specs:
- filename: hootsuite-openapi.yml
  format: yaml
  label: Hootsuite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hootsuite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hootsuite secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hootsuite
provider_slug: hootsuite
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://platform.hootsuite.com/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://platform.hootsuite.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/hootsuite-openapi.yml
  type: oauth2
slug: hootsuite-authentication
source_filename: hootsuite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hootsuite-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.hootsuite.com/oauth2/auth\n    tokenUrl: https://platform.hootsuite.com/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/hootsuite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/authentication/hootsuite-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Social Media
- Social Media Management
- Marketing
- Content Scheduling
- Analytics
- Engagement
---
