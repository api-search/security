---
api_key_in: []
api_specs:
- filename: zuva-classification-api-openapi.yml
  format: yaml
  label: Zuva Classification API
  slug: zuva-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-classification-api-openapi.yml
- filename: zuva-field-extraction-api-openapi.yml
  format: yaml
  label: Zuva Field Extraction API
  slug: zuva-field-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-field-extraction-api-openapi.yml
- filename: zuva-fields-api-openapi.yml
  format: yaml
  label: Zuva Fields API
  slug: zuva-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-fields-api-openapi.yml
- filename: zuva-files-api-openapi.yml
  format: yaml
  label: Zuva Files API
  slug: zuva-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-files-api-openapi.yml
- filename: zuva-ocr-api-openapi.yml
  format: yaml
  label: Zuva OCR API
  slug: zuva-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-ocr-api-openapi.yml
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
- Artificial Intelligence
- Document AI
- Contract Analysis
- Field Extraction
- Classification
- OCR
---
