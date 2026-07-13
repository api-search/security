---
api_key_in: []
api_specs:
- filename: pdfendpoint-openapi.yml
  format: yaml
  label: PDFEndpoint Convert HTML API
  slug: convert-html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/openapi/pdfendpoint-openapi.yml
- filename: pdfendpoint-openapi.yml
  format: yaml
  label: PDFEndpoint Convert URL API
  slug: convert-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/openapi/pdfendpoint-openapi.yml
- filename: pdfendpoint-openapi.yml
  format: yaml
  label: PDFEndpoint Renders and Delivery API
  slug: renders-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/openapi/pdfendpoint-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pdfendpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDFEndpoint secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDFEndpoint
provider_slug: pdfendpoint
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header. Manage keys at https://pdfendpoint.com/app/tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pdfendpoint-openapi.yml
  type: http
slug: pdfendpoint-authentication
source_filename: pdfendpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdfendpoint-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header. Manage keys at\n    https://pdfendpoint.com/app/tokens.\n  sources:\n  - openapi/pdfendpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/authentication/pdfendpoint-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- HTML to PDF
- URL to PDF
- Document Generation
- Conversion
---
