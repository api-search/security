---
api_key_in: []
api_specs:
- filename: taste-health-api-openapi.yml
  format: yaml
  label: Taste health API
  slug: taste-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-health-api-openapi.yml
- filename: taste-prompt-enhancement-api-openapi.yml
  format: yaml
  label: Taste Prompt Enhancement API
  slug: taste-prompt-enhancement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-prompt-enhancement-api-openapi.yml
- filename: taste-taste-engine-api-api-openapi.yml
  format: yaml
  label: Taste Taste Engine API API
  slug: taste-taste-engine-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-taste-engine-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Taste Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taste secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Taste
provider_slug: taste
scheme_count: 1
schemes:
- evidence:
  - detail: 'Authentication required. Provide Authorization: Bearer <token> header.'
    source: live 401 on https://api.tastelabs.com/
  - detail: each operation declares an optional Authorization header parameter
    source: openapi/taste-taste-engine-openapi.json
  format: Bearer <token>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/taste-taste-engine-openapi.json
  type: http
slug: taste-authentication
source_filename: taste-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.tastelabs.com/ (live probe) + openapi/taste-taste-engine-openapi.json\ndocs: null\nnote: >-\n  The published OpenAPI declares no components.securitySchemes, but the live API\n  gateway (https://api.tastelabs.com/) rejects unauthenticated requests with\n  HTTP 401 and the body {\"detail\":\"Authentication required. Provide\n  Authorization: Bearer <token> header.\"}. Every operation also accepts an\n  optional `Authorization` request header. Auth is therefore HTTP Bearer,\n  observed at runtime rather than formally declared in the spec.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: Bearer <token>\n    evidence:\n      - source: live 401 on https://api.tastelabs.com/\n        detail: 'Authentication required. Provide Authorization: Bearer <token> header.'\n\
  \      - source: openapi/taste-taste-engine-openapi.json\n        detail: each operation declares an optional Authorization header parameter\n    sources: [openapi/taste-taste-engine-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/authentication/taste-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Design
- Machine-Learning
- Developer Tools
- Prompt Engineering
- Content Generation
---
