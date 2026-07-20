---
api_key_in:
- header
api_specs:
- filename: defacto-openapi-original.json
  format: json
  label: Defacto API
  slug: defacto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/openapi/defacto-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Defacto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Defacto secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Defacto
provider_slug: defacto
scheme_count: 1
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/defacto-openapi-original.json
  type: apiKey
slug: defacto-authentication
source_filename: defacto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/defacto-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/defacto-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defacto/refs/heads/main/authentication/defacto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- Working Capital
- Invoice Financing
- Credit
- B2B Payments
- SMB
- France
- Europe
---
