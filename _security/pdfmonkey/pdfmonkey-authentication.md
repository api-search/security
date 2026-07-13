---
api_key_in: []
api_specs:
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Document Cards API
  slug: document-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
- filename: pdfmonkey-openapi.yml
  format: yaml
  label: PDFMonkey Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/openapi/pdfmonkey-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pdfmonkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: PDFMonkey secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PDFMonkey
provider_slug: pdfmonkey
scheme_count: 1
schemes:
- description: Pass your secret API key from the dashboard as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pdfmonkey-openapi.yml
  type: http
slug: pdfmonkey-authentication
source_filename: pdfmonkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdfmonkey-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Pass your secret API key from the dashboard as a Bearer token in the Authorization\n    header.\n  sources:\n  - openapi/pdfmonkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/authentication/pdfmonkey-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- Document Generation
- Templates
- HTML to PDF
- Documents
---
