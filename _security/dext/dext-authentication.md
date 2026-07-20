---
api_key_in: []
api_specs:
- filename: dext-data-health-openapi.yml
  format: yaml
  label: Dext Data Health & Insights API
  slug: dext-data-health-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dext/refs/heads/main/openapi/dext-data-health-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Dext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dext secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dext
provider_slug: dext
scheme_count: 1
schemes:
- description: 'Practice-scoped API token sent as `Authorization: Bearer <token>`. Tokens are created and managed in the Dext web app under Practice settings > Data Health > API tokens. The token value is displayed once on creation in a modal and cannot be retrieved afterwards, so it must be stored securely.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dext-data-health-openapi.yml
  type: http
slug: dext-authentication
source_filename: dext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.dext.com/en/articles/272702-data-health-insights-api\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Practice-scoped API token sent as `Authorization: Bearer <token>`. Tokens\n    are created and managed in the Dext web app under Practice settings > Data\n    Health > API tokens. The token value is displayed once on creation in a\n    modal and cannot be retrieved afterwards, so it must be stored securely.\n  sources: [openapi/dext-data-health-openapi.yml]\nnotes: >-\n  The public Data Health & Insights API uses static practice-scoped bearer\n  tokens, not OAuth 2.0 (there is no documented authorization/token endpoint or\n  scope surface for this API). Dext's product-level partner integrations with\n  accounting platforms use their own OAuth flows, but those are not part of the\n  documented\
  \ public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dext/refs/heads/main/authentication/dext-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Accounting
- Bookkeeping
- Receipts
- Expense Management
- Financial Automation
- Data Health
- OCR
---
