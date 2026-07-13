---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: DocSpring API
  slug: docspring-api
  spec_type: OpenAPI
  url: https://docspring.com/api-docs/v1/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docspring Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocSpring secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DocSpring
provider_slug: docspring
scheme_count: 1
schemes:
- description: 'Username: API Token ID, Password: API Token Secret'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/docspring-docspring-api-openapi.yml
  type: http
slug: docspring-authentication
source_filename: docspring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docspring-docspring-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Username: API Token ID, Password: API Token Secret'\n  sources:\n  - openapi/docspring-docspring-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/authentication/docspring-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- Document Generation
- PDF Templates
- E-Signatures
- Forms
- HTML to PDF
- Document Automation
---
