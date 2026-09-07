---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: DietlyAPI
  slug: dietlyapi
  spec_type: OpenAPI
  url: https://www.getdietly.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dietlyapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: DietlyAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DietlyAPI
provider_slug: dietlyapi
scheme_count: 1
schemes:
- description: Optional for the endpoints in this spec. Get a free key instantly at https://www.getdietly.com/account (no card required).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dietlyapi-openapi.json
  type: http
slug: dietlyapi-authentication
source_filename: dietlyapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://www.getdietly.com/developers/api-key-security/ + https://www.getdietly.com/api-guide\ndocs: https://www.getdietly.com/developers/api-key-security/\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional for the endpoints in this spec. Get a free key instantly at https://www.getdietly.com/account\n    (no card required).\n  sources:\n  - openapi/dietlyapi-openapi.json\ndetails:\n  optionality: All public read endpoints work anonymously at 30 req/min per IP; sending a Bearer key switches to per-account plan limits and usage reporting.\n  key_scopes:\n    - name: full-access\n      note: Default for server-side use; can call every endpoint the plan allows.\n    - name: read-only\n      note: Can call every GET data endpoint, 403 anywhere else; recommended wherever a key could leak (client-side code, CI logs, notebooks).\n  key_management:\n    - Per-key expiry\
  \ dates and per-key rate caps set in the dashboard.\n    - Key rotation preserves configuration.\n    - The account key (dashboard /auth/ and /billing/ management) is separate from named access keys; using an access key there returns 403.\n    - TOTP two-factor available on the account.\n  error_behavior: 401 {\"detail\":\"Missing or invalid API key\"} is identical for absent header, wrong scheme and unknown key, so keys cannot be probed; auth runs before routing, so unknown paths also 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dietlyapi/refs/heads/main/authentication/dietlyapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Food
- Nutrition
- Barcodes
- open-food-facts
- Health
- Open Data
---
