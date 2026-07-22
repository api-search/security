---
api_key_in:
- header
api_specs:
- filename: windfall-openapi-original.json
  format: json
  label: Windfall API
  slug: windfall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windfall/refs/heads/main/openapi/windfall-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Windfall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windfall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Windfall
provider_slug: windfall
scheme_count: 1
schemes:
- description: Your API token, provided by Windfall and tied to your organization's account. All requests must include this header and must be made over HTTPS. Tokens are issued by Windfall (not self-service); each token carries a set number of usage tokens corresponding to queryable records, with allocation and refresh frequency determined by your purchase order. Sandbox tokens are prefixed with `sandbox_` and are separate from production tokens — a production token on the sandbox endpoint (or vice versa) returns 403.
  in: header
  name: ApiToken
  parameter: X-WF-Auth-Token
  sources:
  - openapi/windfall-openapi-original.json
  type: apiKey
slug: windfall-authentication
source_filename: windfall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/windfall-openapi-original.json\ndocs: https://api-docs.windfall.com/authentication/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: X-WF-Auth-Token\n  description: >-\n    Your API token, provided by Windfall and tied to your organization's account.\n    All requests must include this header and must be made over HTTPS. Tokens are\n    issued by Windfall (not self-service); each token carries a set number of usage\n    tokens corresponding to queryable records, with allocation and refresh frequency\n    determined by your purchase order. Sandbox tokens are prefixed with `sandbox_`\n    and are separate from production tokens — a production token on the sandbox\n    endpoint (or vice versa) returns 403.\n  sources:\n  - openapi/windfall-openapi-original.json\nnotes:\n  self_service: false\n  token_issuance: Issued by Windfall, tied to\
  \ the organization account.\n  sandbox_prefix: sandbox_\n  https_required: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windfall/refs/heads/main/authentication/windfall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Data Enrichment
- Wealth Data
- People Intelligence
- Career Data
- Identity Resolution
- Sales Intelligence
- Marketing
---
