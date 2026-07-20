---
api_key_in: []
api_specs:
- filename: digio-openapi.yml
  format: yaml
  label: Digio eSign API
  slug: digio-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio eMandate (eNACH) API
  slug: digio-emandate-enach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio KYC API
  slug: digio-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio Documents & eStamp API
  slug: digio-documents-estamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Digio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Digio
provider_slug: digio
scheme_count: 1
schemes:
- bearerFormat: null
  name: basicAuth
  note: 'HTTP Basic authentication. Send Authorization: Basic Base64(client_id:client_secret) with Content-Type application/json. The client_id and client_secret are issued per environment (sandbox ext.digio.in and production api.digio.in) from the Digio dashboard.'
  scheme: basic
  sources:
  - openapi/digio-openapi.yml
  - https://documentation.digio.in/
  type: http
slug: digio-authentication
source_filename: digio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/digio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  bearerFormat: null\n  note: >-\n    HTTP Basic authentication. Send Authorization: Basic\n    Base64(client_id:client_secret) with Content-Type application/json. The\n    client_id and client_secret are issued per environment (sandbox\n    ext.digio.in and production api.digio.in) from the Digio dashboard.\n  sources:\n  - openapi/digio-openapi.yml\n  - https://documentation.digio.in/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/authentication/digio-authentication.yml
summary_line: http · 1 scheme
tags:
- eSign
- KYC
- eNACH
- eMandate
- Digital Signature
- India
- Fintech
- Identity Verification
---
