---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dealscanner Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DealScanner secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DealScanner
provider_slug: dealscanner-io
scheme_count: 1
schemes:
- description: API key in the form "dsk_...". Create one at /api/v1/keys.
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/dealscanner-io-openapi.json
  type: http
slug: dealscanner-io-authentication
source_filename: dealscanner-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dealscanner-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key in the form \"dsk_...\". Create one at /api/v1/keys.\n  sources:\n  - openapi/dealscanner-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dealscanner-io/authentication/dealscanner-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real Estate
- Investment
- Brokerage
- Analytics
---
