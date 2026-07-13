---
api_key_in:
- header
api_specs:
- filename: abortion-policy-api-openapi.yml
  format: yaml
  label: Abortion Policy API
  slug: abortion-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/openapi/abortion-policy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Abortion Policy Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abortion Policy API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
scheme_count: 1
schemes:
- description: API key for authentication. Request access at https://www.abortionpolicyapi.com/request-access
  in: header
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/abortion-policy-api-openapi.yml
  type: apiKey
slug: abortion-policy-api-authentication
source_filename: abortion-policy-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abortion-policy-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: token\n  description: API key for authentication. Request access at https://www.abortionpolicyapi.com/request-access\n  sources:\n  - openapi/abortion-policy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/authentication/abortion-policy-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Abortion
- Policies
- Healthcare
- Government
---
