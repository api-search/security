---
api_key_in:
- header
api_specs:
- filename: pdf-co-barcodes-api-openapi.yml
  format: yaml
  label: PDF.co Barcodes API
  slug: pdf-co-barcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-barcodes-api-openapi.yml
- filename: pdf-co-document-file-system-api-openapi.yml
  format: yaml
  label: PDF.co Document, File & System API
  slug: pdf-co-document-file-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-document-file-system-api-openapi.yml
- filename: pdf-co-editing-api-openapi.yml
  format: yaml
  label: PDF.co Editing API
  slug: pdf-co-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-editing-api-openapi.yml
- filename: pdf-co-excel-conversion-api-openapi.yml
  format: yaml
  label: PDF.co Excel Conversion API
  slug: pdf-co-excel-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-excel-conversion-api-openapi.yml
- filename: pdf-co-extraction-api-openapi.yml
  format: yaml
  label: PDF.co Extraction API
  slug: pdf-co-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-extraction-api-openapi.yml
- filename: pdf-co-find-search-api-openapi.yml
  format: yaml
  label: PDF.co Find & Search API
  slug: pdf-co-find-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-find-search-api-openapi.yml
- filename: pdf-co-forms-api-openapi.yml
  format: yaml
  label: PDF.co Forms API
  slug: pdf-co-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-forms-api-openapi.yml
- filename: pdf-co-pages-api-openapi.yml
  format: yaml
  label: PDF.co Pages API
  slug: pdf-co-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-pages-api-openapi.yml
- filename: pdf-co-pdf-conversion-api-openapi.yml
  format: yaml
  label: PDF.co PDF Conversion API
  slug: pdf-co-pdf-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-pdf-conversion-api-openapi.yml
- filename: pdf-co-pdf-merging-splitting-api-openapi.yml
  format: yaml
  label: PDF.co PDF Merging & Splitting API
  slug: pdf-co-pdf-merging-splitting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/openapi/pdf-co-pdf-merging-splitting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pdf Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDF.co secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDF.co
provider_slug: pdf-co
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/pdf-co-openapi.yml
  type: apiKey
slug: pdf-co-authentication
source_filename: pdf-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdf-co-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/pdf-co-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdf-co/refs/heads/main/authentication/pdf-co-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- PDF
- Document Automation
- Artificial Intelligence
- OCR
- Invoice Parsing
- Document Parsing
- Conversion
- Forms
- Barcodes
- E-Signature
---
