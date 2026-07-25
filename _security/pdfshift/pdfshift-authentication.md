---
api_key_in:
- header
api_specs:
- filename: pdfshift-account-api-openapi.yml
  format: yaml
  label: PDFShift account API
  slug: pdfshift-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-account-api-openapi.yml
- filename: pdfshift-convert-api-openapi.yml
  format: yaml
  label: PDFShift Convert API
  slug: pdfshift-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-convert-api-openapi.yml
- filename: pdfshift-credits-api-openapi.yml
  format: yaml
  label: PDFShift credits API
  slug: pdfshift-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-credits-api-openapi.yml
- filename: pdfshift-details-api-openapi.yml
  format: yaml
  label: PDFShift details API
  slug: pdfshift-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-details-api-openapi.yml
- filename: pdfshift-invoices-api-openapi.yml
  format: yaml
  label: PDFShift Invoices API
  slug: pdfshift-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-invoices-api-openapi.yml
- filename: pdfshift-logs-api-openapi.yml
  format: yaml
  label: PDFShift Logs API
  slug: pdfshift-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-logs-api-openapi.yml
- filename: pdfshift-templates-api-openapi.yml
  format: yaml
  label: PDFShift templates API
  slug: pdfshift-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-templates-api-openapi.yml
- filename: pdfshift-usage-api-openapi.yml
  format: yaml
  label: PDFShift usage API
  slug: pdfshift-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfshift/refs/heads/main/openapi/pdfshift-usage-api-openapi.yml
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
