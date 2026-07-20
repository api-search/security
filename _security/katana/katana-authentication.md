---
api_key_in: []
api_specs:
- filename: katana-openapi-original.json
  format: json
  label: Katana API
  slug: katana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/openapi/katana-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Katana Authentication
name_suffix: Authentication
oauth_flows: []
overview: Katana secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Katana
provider_slug: katana
scheme_count: 1
schemes:
- bearer_format: opaque
  description: 'Account-scoped API key issued in the Katana app (Settings > API > API keys), sent as `Authorization: Bearer <api key>`.'
  header: Authorization
  location: header
  management_url: https://factory.katanamrp.com/settings/api
  name: apiKey
  scheme: bearer
  sources:
  - docs
  type: http
  value_prefix: 'Bearer '
slug: katana-authentication
source_filename: katana-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.katanamrp.com/docs/getting-started\ndocs: https://developer.katanamrp.com/reference/api-authentication\nnotes: >-\n  The published OpenAPI (https://api.katanamrp.com/v1/openapi.json) does not\n  declare any securitySchemes; the auth model below is captured from the Katana\n  developer docs. Katana authenticates every request with an account-scoped API\n  key sent as an HTTP Bearer token. Keys are generated in the Katana app under\n  Settings > API > API keys and are server-side only (never expose in a frontend).\n  A missing/incorrect/outdated key returns 401. Requires a Professional plan or higher.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearer_format: opaque\n  location: header\n  header: Authorization\n  value_prefix: 'Bearer '\n  description: >-\n    Account-scoped API key issued in the\
  \ Katana app (Settings > API > API keys),\n    sent as `Authorization: Bearer <api key>`.\n  management_url: https://factory.katanamrp.com/settings/api\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/authentication/katana-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Inventory
- Manufacturing
- ERP
- Supply Chain
- Warehouse Management
- Order Management
---
