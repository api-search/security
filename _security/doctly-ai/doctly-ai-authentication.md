---
api_key_in: []
api_specs:
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Documents Parse API
  slug: doctly-documents-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Extract API
  slug: doctly-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Status and Results API
  slug: doctly-status-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Doctly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doctly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Doctly
provider_slug: doctly-ai
scheme_count: 1
schemes:
- description: 'Bearer API key, sent as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/doctly-ai-openapi.yml
  type: http
slug: doctly-ai-authentication
source_filename: doctly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/doctly-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key, sent as `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/doctly-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/authentication/doctly-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Document Parsing
- PDF
- Markdown
- Data Extraction
- OCR
---
