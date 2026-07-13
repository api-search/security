---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Parseflow API
  slug: parseflow-api
  spec_type: OpenAPI
  url: https://parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Parseflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parseflow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parseflow
provider_slug: parseflow
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/parseflow-openapi.json
  type: apiKey
slug: parseflow-authentication
source_filename: parseflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parseflow-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/parseflow-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/authentication/parseflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Parsing
- PDF
- OCR
- Text Extraction
- Document AI
- Search
- BYOK
- Async Jobs
- Webhooks
- REST
---
