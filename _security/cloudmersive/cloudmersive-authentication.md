---
api_key_in:
- header
api_specs:
- filename: cloudmersive-scan-api-openapi.yml
  format: yaml
  label: Cloudmersive Scan API
  slug: cloudmersive-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/openapi/cloudmersive-scan-api-openapi.yml
- filename: cloudmersive-scancloudstorage-api-openapi.yml
  format: yaml
  label: Cloudmersive ScanCloudStorage API
  slug: cloudmersive-scancloudstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/openapi/cloudmersive-scancloudstorage-api-openapi.yml
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
