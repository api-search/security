---
api_key_in:
- header
api_specs:
- filename: mathpix-image-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Image OCR API
  slug: mathpix-image-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-image-ocr-api-openapi.yml
- filename: mathpix-document-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Document OCR API
  slug: mathpix-document-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-document-ocr-api-openapi.yml
- filename: mathpix-convert-api-openapi.yml
  format: yaml
  label: Mathpix Convert API
  slug: mathpix-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-convert-api-openapi.yml
- filename: mathpix-batch-api-openapi.yml
  format: yaml
  label: Mathpix Batch API
  slug: mathpix-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-batch-api-openapi.yml
- filename: mathpix-strokes-api-openapi.yml
  format: yaml
  label: Mathpix Strokes API
  slug: mathpix-strokes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-strokes-api-openapi.yml
- filename: mathpix-app-tokens-api-openapi.yml
  format: yaml
  label: Mathpix App Tokens API
  slug: mathpix-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-app-tokens-api-openapi.yml
- filename: mathpix-ocr-usage-api-openapi.yml
  format: yaml
  label: Mathpix OCR Usage API
  slug: mathpix-ocr-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-ocr-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mathpix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mathpix secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mathpix
provider_slug: mathpix
scheme_count: 2
schemes:
- in: header
  name: AppKeyAuth
  parameter: app_key
  sources:
  - openapi/mathpix-app-tokens-api-openapi.yml
  - openapi/mathpix-batch-api-openapi.yml
  - openapi/mathpix-convert-api-openapi.yml
  - openapi/mathpix-image-ocr-api-openapi.yml
  - openapi/mathpix-ocr-usage-api-openapi.yml
  - openapi/mathpix-strokes-api-openapi.yml
  type: apiKey
- in: header
  name: AppIdAuth
  parameter: app_id
  sources:
  - openapi/mathpix-batch-api-openapi.yml
  - openapi/mathpix-convert-api-openapi.yml
  - openapi/mathpix-image-ocr-api-openapi.yml
  - openapi/mathpix-ocr-usage-api-openapi.yml
  - openapi/mathpix-strokes-api-openapi.yml
  type: apiKey
slug: mathpix-authentication
source_filename: mathpix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mathpix-app-tokens-api-openapi.yml, openapi/mathpix-batch-api-openapi.yml, openapi/mathpix-convert-api-openapi.yml,\n  openapi/mathpix-image-ocr-api-openapi.yml, openapi/mathpix-ocr-usage-api-openapi.yml, openapi/mathpix-strokes-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppKeyAuth\n  type: apiKey\n  in: header\n  parameter: app_key\n  sources:\n  - openapi/mathpix-app-tokens-api-openapi.yml\n  - openapi/mathpix-batch-api-openapi.yml\n  - openapi/mathpix-convert-api-openapi.yml\n  - openapi/mathpix-image-ocr-api-openapi.yml\n  - openapi/mathpix-ocr-usage-api-openapi.yml\n  - openapi/mathpix-strokes-api-openapi.yml\n- name: AppIdAuth\n  type: apiKey\n  in: header\n  parameter: app_id\n  sources:\n  - openapi/mathpix-batch-api-openapi.yml\n  - openapi/mathpix-convert-api-openapi.yml\n  - openapi/mathpix-image-ocr-api-openapi.yml\n  - openapi/mathpix-ocr-usage-api-openapi.yml\n\
  \  - openapi/mathpix-strokes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/authentication/mathpix-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- OCR
- STEM
- Math
- Chemistry
- Document Conversion
- PDF
- LaTeX
- Handwriting
- AI
- Machine Learning
---
