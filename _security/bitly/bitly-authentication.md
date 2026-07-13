---
api_key_in: []
api_specs:
- filename: v4.json
  format: json
  label: Bitly API v4
  slug: bitly-api
  spec_type: OpenAPI
  url: https://dev.bitly.com/v4/v4.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bitly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitly
provider_slug: bitly
scheme_count: 1
schemes:
- description: 'Bearer token issued from Bitly account settings, or obtained via OAuth 2.0.

    Send as `Authorization: Bearer {token}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bitly-openapi.yml
  type: http
slug: bitly-authentication
source_filename: bitly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token issued from Bitly account settings, or obtained via OAuth 2.0.\n    Send as `Authorization: Bearer {token}`.\n  sources:\n  - openapi/bitly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/authentication/bitly-authentication.yml
summary_line: http · 1 scheme
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
---
