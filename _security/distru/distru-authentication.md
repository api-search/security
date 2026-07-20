---
api_key_in: []
api_specs:
- filename: distru-openapi.yml
  format: yaml
  label: Distru Public API
  slug: distru-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distru/refs/heads/main/openapi/distru-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Distru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Distru secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Distru
provider_slug: distru
scheme_count: 1
schemes:
- description: 'API key issued in the Distru app under Settings > Integrations > Distru API, sent as `Authorization: Bearer <API_KEY>`. Keys expire one year from issue date.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/distru-openapi.yml
  type: http
slug: distru-authentication
source_filename: distru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/distru-openapi.yml\ndocs: https://help.distru.com/en/articles/12314293-distru-api-faq\nnotes: >-\n  Single scheme: a Bearer API key generated in the Distru app under Settings >\n  Integrations > Distru API. Keys expire one year from issue date. No OAuth,\n  OpenID Connect, or scopes surface. There is no separate sandbox/test mode.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued in the Distru app under Settings > Integrations > Distru API,\n    sent as `Authorization: Bearer <API_KEY>`. Keys expire one year from issue date.'\n  sources:\n  - openapi/distru-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distru/refs/heads/main/authentication/distru-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cannabis
- ERP
- Seed-to-Sale
- Inventory
- Compliance
- Distribution
- Manufacturing
- Wholesale
- Metrc
---
