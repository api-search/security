---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Contently Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Contently secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Contently
provider_slug: contently
scheme_count: 1
schemes:
- description: The Contently Talent API authenticates with scoped OAuth2 access tokens. Per-route rate limits are applied. Exact scope names and token/authorization endpoints are published behind the developer portal (developer.contently.com); the marketing/API docs describe the model as "OAuth2 (scoped)".
  name: OAuth2
  sources:
  - https://contently.com/platform/talent-api/
  type: oauth2
slug: contently-authentication
source_filename: contently-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://contently.com/platform/talent-api/\ndocs: https://developer.contently.com\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  scoped: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The Contently Talent API authenticates with scoped OAuth2 access tokens. Per-route rate limits are\n    applied. Exact scope names and token/authorization endpoints are published behind the developer\n    portal (developer.contently.com); the marketing/API docs describe the model as \"OAuth2 (scoped)\".\n  sources:\n  - https://contently.com/platform/talent-api/\nnotes: >-\n  No OpenAPI/Swagger specification is published (developer.contently.com is a JavaScript single-page app;\n  openapi.json / swagger.json return 404), so scheme detail is captured from published API documentation\n  rather than derived from a machine-readable spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contently/refs/heads/main/authentication/contently-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Content Marketing
- Talent Marketplace
- Freelance
- Content Creation
- Publishing
- Editorial Workflow
- API
---
