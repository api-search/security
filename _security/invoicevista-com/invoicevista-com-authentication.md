---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: InvoiceVista Authentication
name_suffix: Authentication
oauth_flows: []
overview: InvoiceVista secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: InvoiceVista
provider_slug: invoicevista-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key secret>)`.'
  name: apiKey
  scheme: basic
  sources:
  - openapi/invoicevista-com-openapi.json
  type: http
- description: 'Operator session token issued by the InvoiceVista dashboard: `Authorization: Token <access token>`.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/invoicevista-com-openapi.json
  type: apiKey
slug: invoicevista-com-authentication
source_filename: invoicevista-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/invoicevista-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: `Authorization: Basic base64(<key\n    secret>)`.'\n  sources:\n  - openapi/invoicevista-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the InvoiceVista dashboard: `Authorization:\n    Token <access token>`.'\n  sources:\n  - openapi/invoicevista-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/invoicevista-com/authentication/invoicevista-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Invoicing
- Online Invoicing
- Small Business
- Payments
- Multi-Currency
- Financial Analytics
- Data Import
---
