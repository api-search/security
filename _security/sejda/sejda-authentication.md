---
api_key_in:
- header
api_specs:
- filename: sejda-openapi.yml
  format: yaml
  label: Sejda HTML to PDF API
  slug: sejda-html-to-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/openapi/sejda-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sejda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sejda secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sejda
provider_slug: sejda
scheme_count: 1
schemes:
- description: 'Secret API key sent as `Authorization: Token: api_YOURAPIKEYHERE`. A publishable key (`api_public_...`) may be used for browser-side requests when the calling domain is on the account''s allowed-domains list.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/sejda-openapi.yml
  type: apiKey
slug: sejda-authentication
source_filename: sejda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sejda-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Secret API key sent as `Authorization: Token: api_YOURAPIKEYHERE`. A publishable\n    key (`api_public_...`) may be used for browser-side requests when the calling domain is\n    on the account''s allowed-domains list.'\n  sources:\n  - openapi/sejda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/authentication/sejda-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- PDF
- Document Conversion
- HTML to PDF
- PDF Editing
- OCR
---
