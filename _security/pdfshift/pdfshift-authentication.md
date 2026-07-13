---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: PDFShift API
  slug: pdfshift-api
  spec_type: OpenAPI
  url: https://api.pdfshift.io/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pdfshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDFShift secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDFShift
provider_slug: pdfshift
scheme_count: 1
schemes:
- description: 'Authenticate your account by including your secret key in API requests.

    You can manage your API keys in the [Dashboard](https://app.pdfshift.io/dashboard/).


    Authentication to the API is performed by using the HTTP Header X-API-Key.'
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/pdfshift-openapi.json
  type: apiKey
slug: pdfshift-authentication
source_filename: pdfshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdfshift-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    Authenticate your account by including your secret key in API requests.\n    You can manage your API keys in the [Dashboard](https://app.pdfshift.io/dashboard/).\n\n    Authentication to the API is performed by using the HTTP Header X-API-Key.\n  sources:\n  - openapi/pdfshift-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/authentication/pdfshift-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- PDF
- HTML to PDF
- Document Conversion
- Screenshot
- Chromium
- REST API
---
