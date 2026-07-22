---
api_key_in: []
api_specs:
- filename: priorlabs-openapi-original.json
  format: json
  label: TabPFN API
  slug: tabpfn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/priorlabs/refs/heads/main/openapi/priorlabs-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Priorlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prior Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prior Labs
provider_slug: priorlabs
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token for authentication, obtained after signing up and generating an API key.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/priorlabs-openapi-original.json
  type: http
slug: priorlabs-authentication
source_filename: priorlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/priorlabs-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token for authentication, obtained after signing up and generating an\n    API key.\n  sources:\n  - openapi/priorlabs-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/priorlabs/refs/heads/main/authentication/priorlabs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Machine Learning
- Artificial Intelligence
- Tabular Data
- Foundation Models
- Predictions
- Data Science
- MCP
- SDK
---
