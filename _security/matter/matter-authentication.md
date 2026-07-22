---
api_key_in: []
api_specs:
- filename: matter-openapi-original.yml
  format: yaml
  label: Matter API
  slug: matter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matter/refs/heads/main/openapi/matter-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Matter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Matter
provider_slug: matter
scheme_count: 1
schemes:
- description: Personal API token with `mat_` prefix. Generate one at https://web.getmatter.com/settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/matter-openapi-original.yml
  type: http
slug: matter-authentication
source_filename: matter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/matter-openapi-original.yml\ndocs: https://docs.getmatter.com/api/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nmodel: >-\n  Single personal access token per account, passed as an HTTP Bearer token in\n  the Authorization header on every request. Tokens carry the `mat_` prefix and\n  grant full read/write access to the owner's library. Only one token is active\n  at a time — generating or regenerating immediately revokes the previous token.\n  There are no OAuth flows, refresh tokens, or scopes. Every request also\n  requires an active Matter Pro subscription (403 pro_required otherwise).\ntoken:\n  prefix: mat_\n  generate_at: https://web.getmatter.com/settings\n  one_active_token: true\n  rotation: Generating a new token immediately revokes the previous one.\nrequires_subscription: Matter Pro\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal API token\
  \ with `mat_` prefix. Generate one at https://web.getmatter.com/settings.\n  sources:\n  - openapi/matter-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matter/refs/heads/main/authentication/matter-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Reading
- Read Later
- Productivity
- Content
- Highlights
- Bookmarking
---
