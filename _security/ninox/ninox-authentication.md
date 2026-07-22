---
api_key_in: []
api_specs:
- filename: ninox-public-openapi-original.json
  format: json
  label: Ninox Public API
  slug: ninox-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/openapi/ninox-public-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ninox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ninox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ninox
provider_slug: ninox
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: "Enter your Workspace API key. \n\n API keys can be generated and managed within the **Workspace Integration** settings in the Ninox app."
  name: bearer
  scheme: bearer
  sources:
  - openapi/ninox-public-openapi-original.json
  type: http
slug: ninox-authentication
source_filename: ninox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ninox-public-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: \"Enter your Workspace API key. \\n\\n API keys can be generated and managed within\\\n    \\ the **Workspace Integration** settings in the Ninox app.\"\n  sources:\n  - openapi/ninox-public-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/authentication/ninox-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Low-Code
- Database
- No-Code
- Application Development
- Workflow Automation
- Business Apps
- Productivity
---
