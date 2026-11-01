---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cloudmersive-imageocr-api-openapi.yml
  format: yaml
  label: Cloudmersive Image Ocr API
  slug: cloudmersive-imageocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmersive/openapi/cloudmersive-imageocr-api-openapi.yml
- filename: cloudmersive-pdfocr-api-openapi.yml
  format: yaml
  label: Cloudmersive PDF Ocr API
  slug: cloudmersive-pdfocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmersive/openapi/cloudmersive-pdfocr-api-openapi.yml
- filename: cloudmersive-preprocessing-api-openapi.yml
  format: yaml
  label: Cloudmersive Preprocessing API
  slug: cloudmersive-preprocessing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmersive/openapi/cloudmersive-preprocessing-api-openapi.yml
- filename: cloudmersive-receipts-api-openapi.yml
  format: yaml
  label: Cloudmersive Receipts API
  slug: cloudmersive-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudmersive/openapi/cloudmersive-receipts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cloudmersive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudmersive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudmersive
provider_slug: cloudmersive
scheme_count: 1
schemes:
- description: API Key Authentication
  in: header
  name: Apikey
  parameter: Apikey
  sources:
  - openapi/cloudmersive-virus-scan-openapi.json
  type: apiKey
slug: cloudmersive-authentication
source_filename: cloudmersive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudmersive-virus-scan-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Apikey\n  type: apiKey\n  in: header\n  parameter: Apikey\n  description: API Key Authentication\n  sources:\n  - openapi/cloudmersive-virus-scan-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cloudmersive/authentication/cloudmersive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Barcodes
- Conversion
- Documents
- Image Recognition
- Natural-Language
- OCR
- Processing
- Validation
- Virus Scanning
---
