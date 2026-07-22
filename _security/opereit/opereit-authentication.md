---
api_key_in: []
api_specs:
- filename: opereit-invoice-auditing-openapi.json
  format: json
  label: Opereit Invoice Auditing API
  slug: opereit-invoice-auditing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opereit/refs/heads/main/openapi/opereit-invoice-auditing-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opereit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opereit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opereit
provider_slug: opereit
scheme_count: 1
schemes:
- description: 'HTTP Basic Auth using your API key. Send `Authorization: Basic base64(key_id:key_secret)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/opereit-invoice-auditing-openapi.json
  type: http
slug: opereit-authentication
source_filename: opereit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opereit-invoice-auditing-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Auth using your API key. Send `Authorization: Basic base64(key_id:key_secret)`.'\n  sources:\n  - openapi/opereit-invoice-auditing-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opereit/refs/heads/main/authentication/opereit-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Supply Chain
- Shipping
- Invoice Auditing
- Cost Recovery
- Freight Audit
- Artificial Intelligence
- AI Agents
---
