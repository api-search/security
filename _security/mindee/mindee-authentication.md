---
api_key_in:
- header
api_specs:
- filename: mindee-extraction-api-openapi.yml
  format: yaml
  label: Mindee Extraction API
  slug: mindee-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-extraction-api-openapi.yml
- filename: mindee-classification-api-openapi.yml
  format: yaml
  label: Mindee Classification API
  slug: mindee-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-classification-api-openapi.yml
- filename: mindee-crop-api-openapi.yml
  format: yaml
  label: Mindee Crop API
  slug: mindee-crop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-crop-api-openapi.yml
- filename: mindee-ocr-api-openapi.yml
  format: yaml
  label: Mindee OCR API
  slug: mindee-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-ocr-api-openapi.yml
- filename: mindee-split-api-openapi.yml
  format: yaml
  label: Mindee Split API
  slug: mindee-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-split-api-openapi.yml
- filename: mindee-jobs-api-openapi.yml
  format: yaml
  label: Mindee Jobs API
  slug: mindee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-jobs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mindee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mindee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mindee
provider_slug: mindee
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/mindee-classification-api-openapi.yml
  - openapi/mindee-crop-api-openapi.yml
  - openapi/mindee-extraction-api-openapi.yml
  - openapi/mindee-jobs-api-openapi.yml
  - openapi/mindee-ocr-api-openapi.yml
  - openapi/mindee-split-api-openapi.yml
  type: apiKey
slug: mindee-authentication
source_filename: mindee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mindee-classification-api-openapi.yml, openapi/mindee-crop-api-openapi.yml,\n  openapi/mindee-extraction-api-openapi.yml, openapi/mindee-jobs-api-openapi.yml, openapi/mindee-ocr-api-openapi.yml,\n  openapi/mindee-split-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/mindee-classification-api-openapi.yml\n  - openapi/mindee-crop-api-openapi.yml\n  - openapi/mindee-extraction-api-openapi.yml\n  - openapi/mindee-jobs-api-openapi.yml\n  - openapi/mindee-ocr-api-openapi.yml\n  - openapi/mindee-split-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/authentication/mindee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Parsing
- OCR
- IDP
- AI
- Machine Learning
- Invoices
- Receipts
- IDs
- Computer Vision
---
