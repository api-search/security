---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: erechio-pr-fen-api-openapi.yml
  format: yaml
  label: Erechio Prüfen API
  slug: erechio-pr-fen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erechio/openapi/erechio-pr-fen-api-openapi.yml
- filename: erechio-status-api-openapi.yml
  format: yaml
  label: Erechio Status API
  slug: erechio-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erechio/openapi/erechio-status-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Erechio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Erechio secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Erechio
provider_slug: erechio
scheme_count: 2
schemes:
- description: 'Header `Authorization: Bearer pk_…`'
  name: bearer
  scheme: bearer
  sources:
  - openapi/erechio-openapi.json
  type: http
- description: Alternativ zum Bearer-Header
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/erechio-openapi.json
  type: apiKey
slug: erechio-authentication
source_filename: erechio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/erechio-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Header `Authorization: Bearer pk_…`'\n  sources:\n  - openapi/erechio-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternativ zum Bearer-Header\n  sources:\n  - openapi/erechio-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/erechio/authentication/erechio-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- German
- e-invoice
- Validation
- XRechnung
- ZUGFeRD
- KoSIT
---
