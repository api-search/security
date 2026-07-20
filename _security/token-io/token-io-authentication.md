---
api_key_in:
- header
api_specs:
- filename: token-io-openapi.yml
  format: yaml
  label: Token.io Open Banking API
  slug: token-io-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/openapi/token-io-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Token Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: token-io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: token-io
provider_slug: token-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: '**For Production and Sandbox environments.**<br />When using curl samples the authorization header is given as -H `''Authorization: Bearer + JWT''`<br/>Please substitute your Bearer key here.<br/>For example:<br/> -H `''Authorization: Bearer [example key]'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/token-io-openapi.yml
  type: http
- description: '**For Sandbox environment only.**<br />When using curl samples the authorization header is given as -H `''Authorization: YOUR_API_KEY_HERE''`<br/>Please substitute your Basic key here.<br/>For example:<br/> -H `''Authorization: Basic [example key]''`'
  in: header
  name: BasicAuth
  parameter: Authorization
  sources:
  - openapi/token-io-openapi.yml
  type: apiKey
slug: token-io-authentication
source_filename: token-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/token-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: '**For Production and Sandbox environments.**<br />When using curl samples the\n    authorization header is given as -H `''Authorization: Bearer + JWT''`<br/>Please substitute\n    your Bearer key here.<br/>For example:<br/> -H `''Authorization: Bearer [example key]'\n  sources:\n  - openapi/token-io-openapi.yml\n- name: BasicAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '**For Sandbox environment only.**<br />When using curl samples the authorization\n    header is given as -H `''Authorization: YOUR_API_KEY_HERE''`<br/>Please substitute your\n    Basic key here.<br/>For example:<br/> -H `''Authorization: Basic [example key]''`'\n  sources:\n  - openapi/token-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/token-io/refs/heads/main/authentication/token-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
