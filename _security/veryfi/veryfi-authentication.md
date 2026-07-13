---
api_key_in:
- header
api_specs:
- filename: veryfi-ocr-openapi.yml
  format: yaml
  label: Veryfi OCR API
  slug: ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-ocr-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veryfi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veryfi secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Veryfi
provider_slug: veryfi
scheme_count: 3
schemes:
- description: Your Veryfi account client identifier
  in: header
  name: clientId
  parameter: CLIENT-ID
  sources:
  - openapi/veryfi-ocr-openapi.yml
  type: apiKey
- description: 'API key in format: ''apikey USERNAME:API_KEY'''
  in: header
  name: apiKey
  parameter: AUTHORIZATION
  sources:
  - openapi/veryfi-ocr-openapi.yml
  type: apiKey
- description: HMAC-SHA256 signature for request validation
  in: header
  name: requestSignature
  parameter: X-Veryfi-Request-Signature
  sources:
  - openapi/veryfi-ocr-openapi.yml
  type: apiKey
slug: veryfi-authentication
source_filename: veryfi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veryfi-ocr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: CLIENT-ID\n  description: Your Veryfi account client identifier\n  sources:\n  - openapi/veryfi-ocr-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: AUTHORIZATION\n  description: 'API key in format: ''apikey USERNAME:API_KEY'''\n  sources:\n  - openapi/veryfi-ocr-openapi.yml\n- name: requestSignature\n  type: apiKey\n  in: header\n  parameter: X-Veryfi-Request-Signature\n  description: HMAC-SHA256 signature for request validation\n  sources:\n  - openapi/veryfi-ocr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/authentication/veryfi-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- AI
- Document Processing
- Finance
- Invoices
- OCR
- Receipts
- Tax Forms
---
