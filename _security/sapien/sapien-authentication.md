---
api_key_in: []
api_specs:
- filename: sapien-poq-openapi-original.json
  format: json
  label: Sapien Proof of Quality Developer API
  slug: sapien-proof-of-quality-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sapien/refs/heads/main/openapi/sapien-poq-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sapien Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sapien secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sapien
provider_slug: sapien
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'Developer API key using the Authorization: Bearer poq_live_... header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sapien-poq-openapi-original.json
  type: http
slug: sapien-authentication
source_filename: sapien-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sapien-poq-openapi-original.json\ndocs: https://docs.sapien.io/integrate/api-keys\nsummary:\n  types:\n  - http\n  api_key_format: poq_live_ + 32 base62 chars (41 chars total)\n  key_management: https://sapien-poq.up.railway.app/originator/api-keys\n  note: >-\n    Token is shown exactly once at creation and cannot be retrieved later. Project and\n    upload endpoints additionally require the key creator to be an org originator.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Developer API key using the Authorization: Bearer poq_live_... header.'\n  sources:\n  - openapi/sapien-poq-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapien/refs/heads/main/authentication/sapien-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Data Quality
- Data Labeling
- Machine Learning
- Human in the Loop
- Attestation
- Blockchain
- Consensus
- MCP
---
