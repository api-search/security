---
api_key_in:
- header
api_specs:
- filename: nace-ai-ndi-openapi.json
  format: json
  label: Nace Document Intelligence (NDI)
  slug: nace-document-intelligence-ndi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nace-ai/refs/heads/main/openapi/nace-ai-ndi-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nace Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nace Ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nace Ai
provider_slug: nace-ai
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nace-ai-ndi-openapi.json
  type: apiKey
slug: nace-ai-authentication
source_filename: nace-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nace-ai-ndi-openapi.json\ndocs: https://docs.ndi.nace.ai\nkey_prefix: ndi_sk_\nnotes: >-\n  Single-header API key auth. Send X-API-Key: ndi_sk_... on every request (REST\n  and MCP). The MCP integration docs note OAuth support may be added later.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/nace-ai-ndi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nace-ai/refs/heads/main/authentication/nace-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Document Intelligence
- Document Processing
- Data Extraction
- OCR
- Machine Learning
- Enterprise Automation
- MCP
---
