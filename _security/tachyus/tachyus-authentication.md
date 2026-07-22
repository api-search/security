---
api_key_in:
- header
api_specs:
- filename: tachyus-tachapps-openapi.yml
  format: yaml
  label: Tachapps API
  slug: tachapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/openapi/tachyus-tachapps-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tachyus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tachyus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tachyus
provider_slug: tachyus
scheme_count: 1
schemes:
- description: 'Bearer API token sent in the Authorization header as `Authorization: Bearer tach_live_...`. Tokens are generated from the Tachapps UI (Settings -> API Tokens): name the token, optionally set an expiration date, generate and copy it once (not displayable afterward). Tokens can be revoked at any time and should be rotated regularly.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tachyus-tachapps-openapi.yml
  type: http
slug: tachyus-authentication
source_filename: tachyus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tachyus.com/api/authentication.html\ndocs: https://docs.tachyus.com/api/authentication.html\nsummary:\n  types: [http]\n  scheme: bearer\n  token_style: personal-access-token\n  token_prefix: tach_live_\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer API token sent in the Authorization header as\n      `Authorization: Bearer tach_live_...`. Tokens are generated from the\n      Tachapps UI (Settings -> API Tokens): name the token, optionally set an\n      expiration date, generate and copy it once (not displayable afterward).\n      Tokens can be revoked at any time and should be rotated regularly.\n    sources: [openapi/tachyus-tachapps-openapi.yml]\ntoken_management:\n  issue: Settings -> API Tokens -> Generate New Token\n  expiration: optional per-token expiration date\n  revoke: Settings -> API Tokens -> Revoke\n\
  \  storage_guidance: store in environment variables / secrets manager, never in source control\nscopes:\n  - read:projects\n  - read:wells\n  - read:production\n  - write:projects\n  - write:wells\n  - admin\nerrors:\n  - status: 401\n    code: UNAUTHORIZED\n    meaning: Token missing or invalid\n  - status: 403\n    code: FORBIDDEN\n    meaning: Token lacks required scope\n  - status: 429\n    code: RATE_LIMITED\n    meaning: Rate limit exceeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tachyus/refs/heads/main/authentication/tachyus-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Energy
- Oil and Gas
- Reservoir Management
- Production Optimization
- Emissions Management
- Machine Learning
- Analytics
---
