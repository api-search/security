---
api_key_in:
- header
api_specs:
- filename: windfall-data-openapi-original.json
  format: json
  label: Windfall API
  slug: windfall-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windfall-data/refs/heads/main/openapi/windfall-data-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Windfall Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windfall Data secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Windfall Data
provider_slug: windfall-data
scheme_count: 1
schemes:
- description: Your API token, provided by Windfall. All requests must include this header.
  in: header
  name: ApiToken
  parameter: X-WF-Auth-Token
  sources:
  - openapi/windfall-data-openapi-original.json
  type: apiKey
slug: windfall-data-authentication
source_filename: windfall-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/windfall-data-openapi-original.json\ndocs: https://api-docs.windfall.com/authentication/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  note: >-\n    Static organization-scoped token issued by Windfall, sent in the X-WF-Auth-Token\n    header over HTTPS. Production and sandbox tokens are separate and non-interchangeable\n    (sandbox tokens are prefixed sandbox_). No OAuth or scopes.\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-WF-Auth-Token\n  description: Your API token, provided by Windfall. All requests must include this header.\n  sources:\n  - openapi/windfall-data-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windfall-data/refs/heads/main/authentication/windfall-data-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Data Enrichment
- Wealth Data
- People Intelligence
- Net Worth
- Identity Resolution
- Marketing
- Sales
---
