---
api_key_in:
- header
api_specs:
- filename: veryfi-any-documents-api-openapi.yml
  format: yaml
  label: Veryfi Any Documents API
  slug: veryfi-any-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-any-documents-api-openapi.yml
- filename: veryfi-bank-statements-api-openapi.yml
  format: yaml
  label: Veryfi Bank Statements API
  slug: veryfi-bank-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-bank-statements-api-openapi.yml
- filename: veryfi-checks-api-openapi.yml
  format: yaml
  label: Veryfi Checks API
  slug: veryfi-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-checks-api-openapi.yml
- filename: veryfi-classification-api-openapi.yml
  format: yaml
  label: Veryfi Classification API
  slug: veryfi-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-classification-api-openapi.yml
- filename: veryfi-documents-api-openapi.yml
  format: yaml
  label: Veryfi Documents API
  slug: veryfi-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-documents-api-openapi.yml
- filename: veryfi-w-2-forms-api-openapi.yml
  format: yaml
  label: Veryfi W-2 Forms API
  slug: veryfi-w-2-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-w-2-forms-api-openapi.yml
- filename: veryfi-w-9-forms-api-openapi.yml
  format: yaml
  label: Veryfi W-9 Forms API
  slug: veryfi-w-9-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veryfi/refs/heads/main/openapi/veryfi-w-9-forms-api-openapi.yml
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
- Artificial Intelligence
- Document Processing
- Finance
- Invoices
- OCR
- Receipts
- Tax Forms
---
