---
api_key_in:
- header
api_specs:
- filename: posit-connect-openapi-original.json
  format: json
  label: Posit Connect Server API
  slug: posit-connect-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posit/refs/heads/main/openapi/posit-connect-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Posit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Posit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Posit
provider_slug: posit
scheme_count: 1
schemes:
- description: Prefix your API key with `Key `, e.g. `Key ABC123`.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/posit-connect-openapi-original.json
  type: apiKey
slug: posit-authentication
source_filename: posit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/posit-connect-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Prefix your API key with `Key `, e.g. `Key ABC123`.\n  sources:\n  - openapi/posit-connect-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posit/refs/heads/main/authentication/posit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Science
- Analytics
- Developer Tools
- R
- Python
- Publishing
- Machine Learning
- Enterprise
- Reproducibility
---
