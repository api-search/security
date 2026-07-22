---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Lume Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lume secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lume
provider_slug: lume
scheme_count: 1
schemes:
- description: Per-account API key issued in the Lume application under Settings > API Keys. Sent on every request in the lume-api-key request header. The Python SDK also reads it from the LUME_API_KEY environment variable or via lume.init(api_key=...); the TypeScript SDK takes it in the Lume constructor.
  in: header
  name: LumeApiKey
  parameter_name: lume-api-key
  sources:
  - packages/lume-packages.yml
  - https://docs.lume.ai
  type: apiKey
slug: lume-authentication
source_filename: lume-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.lume.ai/pages/libraries/python-ent/quickstart.md + typescript-sdk BaseService\ndocs: https://docs.lume.ai/pages/documentation/getting_started/quickstart.md\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: LumeApiKey\n  type: apiKey\n  in: header\n  parameter_name: lume-api-key\n  description: >-\n    Per-account API key issued in the Lume application under Settings > API Keys. Sent on every\n    request in the lume-api-key request header. The Python SDK also reads it from the LUME_API_KEY\n    environment variable or via lume.init(api_key=...); the TypeScript SDK takes it in the Lume\n    constructor.\n  sources:\n  - packages/lume-packages.yml\n  - https://docs.lume.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lume/refs/heads/main/authentication/lume-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Integration
- Data Mapping
- ETL
- Data Transformation
- Artificial Intelligence
- Schema Mapping
- Data Quality
- Developer Tools
---
