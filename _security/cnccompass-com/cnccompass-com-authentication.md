---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: cnccompass-com-mcp-api-openapi.yml
  format: yaml
  label: CNC Compass MCP API
  slug: cnccompass-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnccompass-com/openapi/cnccompass-com-mcp-api-openapi.yml
- filename: cnccompass-com-search-api-openapi.yml
  format: yaml
  label: CNC Compass Search API
  slug: cnccompass-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnccompass-com/openapi/cnccompass-com-search-api-openapi.yml
auth_types:
- apiKey
- anonymous
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CNC Compass Authentication
name_suffix: Authentication
oauth_flows: []
overview: CNC Compass secures its APIs with apiKey and anonymous across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CNC Compass
provider_slug: cnccompass-com
scheme_count: 2
schemes:
- description: Anonymous callers are accepted on /api/search and /mcp; they share a per-IP quota (access manifest auth.anonymous true).
  name: anonymous
  sources:
  - https://cnccompass.com/.well-known/ai-access.json
  type: none
- alternate_header: 'Authorization: Bearer <key>'
  description: 'Optional. Raises the anonymous per-IP quota. "A key issued by CNC Compass raises it; Authorization: Bearer is accepted too."'
  in: header
  issuance: Key is issued by CNC Compass; no self-serve key signup is documented.
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/cnccompass-com-openapi.yml
  - https://cnccompass.com/.well-known/ai-access.json
  type: apiKey
slug: cnccompass-com-authentication
source_filename: cnccompass-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cnccompass.com/.well-known/ai-access.json\ndocs: https://cnccompass.com/.well-known/ai-access.json\nsummary:\n  types:\n  - apiKey\n  - anonymous\n  api_key_in:\n  - header\n  optional: true\nschemes:\n- name: anonymous\n  type: none\n  description: Anonymous callers are accepted on /api/search and /mcp; they share a per-IP quota (access manifest auth.anonymous true).\n  sources:\n  - https://cnccompass.com/.well-known/ai-access.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Optional. Raises the anonymous per-IP quota. \"A key issued by CNC Compass raises it; Authorization: Bearer is accepted too.\"'\n  alternate_header: 'Authorization: Bearer <key>'\n  issuance: Key is issued by CNC Compass; no self-serve key signup is documented.\n  sources:\n  - openapi/cnccompass-com-openapi.yml\n  - https://cnccompass.com/.well-known/ai-access.json\n"
source_yaml_url: https://artifacts.apis.io/cnccompass-com/authentication/cnccompass-com-authentication.yml
summary_line: apiKey/anonymous · 2 schemes
tags:
- Company
- CNC Machining
- Manufacturing
- Supplier Search
- Sourcing
- Procurement
- MCP
- SERP
---
