---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invoicecraftly-documents-api-openapi.yml
  format: yaml
  label: InvoiceCraftly Developer Document API Documents API
  slug: invoicecraftly-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoicecraftly/refs/heads/main/openapi/invoicecraftly-documents-api-openapi.yml
- filename: invoicecraftly-structured-invoicing-api-openapi.yml
  format: yaml
  label: InvoiceCraftly Developer Document API Structured invoicing API
  slug: invoicecraftly-structured-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invoicecraftly/refs/heads/main/openapi/invoicecraftly-structured-invoicing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Invoicecraftly Authentication
name_suffix: Authentication
oauth_flows: []
overview: InvoiceCraftly Developer Document API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InvoiceCraftly Developer Document API
provider_slug: invoicecraftly
scheme_count: 1
schemes:
- bearerFormat: dk_live_*
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/invoicecraftly-openapi.json
  type: http
slug: invoicecraftly-authentication
source_filename: invoicecraftly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/invoicecraftly-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: dk_live_*\n  sources:\n  - openapi/invoicecraftly-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invoicecraftly/refs/heads/main/authentication/invoicecraftly-authentication.yml
summary_line: http · 1 scheme
tags:
- Invoicing
- Invoice Generator
- Free Tools
- Document Export
- Payment QR
- No Signup
- CSV Import
- Company Lookup
---
