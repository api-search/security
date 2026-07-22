---
api_key_in: []
api_specs:
- filename: parcha-openapi-original.json
  format: json
  label: Parcha API
  slug: parcha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcha/refs/heads/main/openapi/parcha-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Parcha Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parcha secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parcha
provider_slug: parcha
scheme_count: 1
schemes:
- description: API key obtained from your Parcha account settings. Include as Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parcha-docs-openapi.yaml
  - openapi/parcha-openapi-original.json
  type: http
slug: parcha-authentication
source_filename: parcha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/parcha-docs-openapi.yaml, openapi/parcha-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key obtained from your Parcha account settings. Include as Bearer token in\n    the Authorization header.\n  sources:\n  - openapi/parcha-docs-openapi.yaml\n  - openapi/parcha-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcha/refs/heads/main/authentication/parcha-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise Saas
- Compliance
- KYB
- KYC
- Due Diligence
- AML
- Sanctions Screening
- Identity Verification
- Financial Services
- Artificial Intelligence
---
