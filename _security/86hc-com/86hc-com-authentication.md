---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 86hc-com-openapi.json
  format: json
  label: Hong Kong Company MCP & Corporate Registry API
  slug: hong-kong-company-mcp-corporate-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/86hc-com/openapi/86hc-com-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 恒诚 Authentication
name_suffix: Authentication
oauth_flows: []
overview: 恒诚 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 恒诚
provider_slug: 86hc-com
scheme_count: 1
schemes:
- description: Optional 86hc.com API Key (hkq_live_...). Omit for 3 free company details/day per IP, or obtain a free key at https://www.86hc.com/user for 20 free queries/day.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/86hc-com-openapi.json
  type: apiKey
slug: 86hc-com-authentication
source_filename: 86hc-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/86hc-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional 86hc.com API Key (hkq_live_...). Omit for 3 free company details/day\n    per IP, or obtain a free key at https://www.86hc.com/user for 20 free queries/day.\n  sources:\n  - openapi/86hc-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/86hc-com/authentication/86hc-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hong Kong
- Business Intelligence
- Due Diligence
- Corporate Services
- Compliance
---
