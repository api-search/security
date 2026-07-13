---
api_key_in: []
api_specs:
- filename: duda-partner-api.json
  format: json
  label: Duda Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-partner-api.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Duda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duda
provider_slug: duda
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using API user credentials (base64 encoded user:pass)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/duda-partner-api.json
  type: http
slug: duda-authentication
source_filename: duda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duda-partner-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using API user credentials (base64 encoded user:pass)\n  sources:\n  - openapi/duda-partner-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/authentication/duda-authentication.yml
summary_line: http · 1 scheme
tags:
- Website Builder
- Agencies
- White Label
- SaaS
- eCommerce
- CMS
---
