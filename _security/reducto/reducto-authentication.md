---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Reducto Document API
  slug: reducto-document-api
  spec_type: OpenAPI
  url: https://api.reductoai.com/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reducto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reducto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reducto
provider_slug: reducto
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/reducto-document-api-openapi.yml
  type: http
slug: reducto-authentication
source_filename: reducto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reducto-document-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/reducto-document-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/authentication/reducto-authentication.yml
summary_line: http · 1 scheme
tags:
- Document Parsing
- PDF
- OCR
- Data Extraction
- AI
- Machine Learning
- Document Intelligence
- Structured Data
---
