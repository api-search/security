---
api_key_in: []
api_specs:
- filename: ninetyio-openapi-original.json
  format: json
  label: Ninety Public API
  slug: ninety-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninetyio/refs/heads/main/openapi/ninetyio-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ninetyio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ninety.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ninety.io
provider_slug: ninetyio
scheme_count: 1
schemes:
- bearer_format: JWT
  description: Personal Access Token — generate one at https://app.ninety.io/settings/user/developer-settings
  location: header (Authorization)
  name: JWT
  scheme: bearer
  sources:
  - openapi/ninetyio-openapi-original.json
  type: http
slug: ninetyio-authentication
source_filename: ninetyio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ninetyio-openapi-original.json\ndocs: https://help.ninety.io/en/articles/15505694-api-reference-and-access\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  token_model: personal-access-token\n  oauth2_flows: []\n  api_key_in: []\n  notes: >-\n    Authentication is a Personal Access Token (PAT) passed as an HTTP Bearer\n    token in the Authorization header. Tokens are generated per user at\n    https://app.ninety.io/settings/user/developer-settings with a selectable\n    expiration (30, 90, 180, or 365 days). Every call executes as the generating\n    user and respects that user's in-app permissions; there is no admin or\n    superuser override, and cross-company access requires a separate token per\n    company. There is no OAuth2 / OpenID Connect flow and no scope surface.\nschemes:\n  - name: JWT\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      Personal\
  \ Access Token — generate one at\n      https://app.ninety.io/settings/user/developer-settings\n    location: header (Authorization)\n    sources: [openapi/ninetyio-openapi-original.json]\napplied:\n  global: true\n  requirement: [{JWT: []}]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninetyio/refs/heads/main/authentication/ninetyio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- EOS
- Entrepreneurial Operating System
- Business Management
- Meetings
- Productivity
- Scorecard
- Team Management
- Goal Tracking
---
