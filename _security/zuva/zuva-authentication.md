---
api_key_in: []
api_specs:
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Field Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Classification API
  slug: classification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Language API
  slug: language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva OCR API
  slug: ocr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Fields Catalog API
  slug: fields-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zuva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zuva secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zuva
provider_slug: zuva
scheme_count: 1
schemes:
- description: 'Zuva API token passed in the Authorization header as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zuva-openapi.yml
  type: http
slug: zuva-authentication
source_filename: zuva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zuva-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Zuva API token passed in the Authorization header as `Authorization: Bearer\n    <token>`.'\n  sources:\n  - openapi/zuva-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/authentication/zuva-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Document AI
- Contract Analysis
- Field Extraction
- Classification
- OCR
---
