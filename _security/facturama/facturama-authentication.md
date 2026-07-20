---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Facturama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facturama secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facturama
provider_slug: facturama
scheme_count: 1
schemes:
- description: 'The Facturama API authenticates with HTTP Basic authentication. Clients send an Authorization header of the form "Authorization: Basic <base64(username:password)>", where the credentials are the API user/token pair created in the Facturama account (distinct from the web login). The same scheme is used for the sandbox and production hosts; only the base URL changes.'
  name: BasicAuth
  scheme: basic
  sources:
  - docs
  type: http
slug: facturama-authentication
source_filename: facturama-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apisandbox.facturama.mx/Docs\ndocs: https://apisandbox.facturama.mx/Docs\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    The Facturama API authenticates with HTTP Basic authentication. Clients send an\n    Authorization header of the form \"Authorization: Basic <base64(username:password)>\",\n    where the credentials are the API user/token pair created in the Facturama account\n    (distinct from the web login). The same scheme is used for the sandbox and\n    production hosts; only the base URL changes.\n  sources: [docs]\nnotes:\n- API Web credentials are tied to a single Facturama account/issuer.\n- API Multiemisor uses account-level credentials to invoice on behalf of many taxpayers.\n- No OAuth 2.0 or OpenID Connect surface is documented; there is no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facturama/refs/heads/main/authentication/facturama-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Electronic Invoicing
- CFDI
- e-Invoicing
- Mexico
- Tax Compliance
- SAT
- Billing
- Payroll
- Finance
- REST API
---
