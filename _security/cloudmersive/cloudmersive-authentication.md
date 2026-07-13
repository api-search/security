---
api_key_in:
- header
api_specs:
- filename: virus
  format: yaml
  label: Cloudmersive Virus Scan API
  slug: cloudmersive-virus-scan-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/virus
- filename: security
  format: yaml
  label: Cloudmersive Security Threat Detection API
  slug: cloudmersive-security-threat-detection-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/security
- filename: spam
  format: yaml
  label: Cloudmersive Spam Detection API
  slug: cloudmersive-spam-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/spam
- filename: phishing
  format: yaml
  label: Cloudmersive Phishing Detection API
  slug: cloudmersive-phishing-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/phishing
- filename: cdr
  format: yaml
  label: Cloudmersive Content Disarm and Reconstruction (CDR) API
  slug: cloudmersive-cdr-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/cdr
- filename: fraud
  format: yaml
  label: Cloudmersive Fraud Detection API
  slug: cloudmersive-fraud-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/fraud
- filename: dlp
  format: yaml
  label: Cloudmersive Data Loss Prevention (DLP) API
  slug: cloudmersive-dlp-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/dlp
- filename: convert
  format: yaml
  label: Cloudmersive Document Convert API
  slug: cloudmersive-convert-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/convert
- filename: barcode
  format: yaml
  label: Cloudmersive Barcode API
  slug: cloudmersive-barcode-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/barcode
- filename: image
  format: yaml
  label: Cloudmersive Image Recognition and Processing API
  slug: cloudmersive-image-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/image
- filename: nlp
  format: yaml
  label: Cloudmersive Natural Language Processing API
  slug: cloudmersive-nlp-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/nlp
- filename: ocr
  format: yaml
  label: Cloudmersive OCR API
  slug: cloudmersive-ocr-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/ocr
- filename: speech
  format: yaml
  label: Cloudmersive Speech API
  slug: cloudmersive-speech-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/speech
- filename: validate
  format: yaml
  label: Cloudmersive Validate API
  slug: cloudmersive-validate-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/validate
- filename: video
  format: yaml
  label: Cloudmersive Video API
  slug: cloudmersive-video-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/video
- filename: currency
  format: yaml
  label: Cloudmersive Currency API
  slug: cloudmersive-currency-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/currency
- filename: config
  format: yaml
  label: Cloudmersive Configuration API
  slug: cloudmersive-config-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/config
- filename: dataintegration
  format: yaml
  label: Cloudmersive Data Integration API
  slug: cloudmersive-data-integration-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/dataintegration
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/authentication/cloudmersive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Barcodes
- Conversions
- Documents
- Image Recognition
- Natural Language
- OCR
- Processing
- Validation
- Virus Scanning
---
