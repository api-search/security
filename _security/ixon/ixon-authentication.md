---
api_key_in: []
api_specs:
- filename: ixon-openapi.json
  format: json
  label: IXON Cloud API
  slug: ixon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ixon/refs/heads/main/openapi/ixon-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ixon Authentication
name_suffix: Authentication
oauth_flows: []
overview: IXON secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IXON
provider_slug: ixon
scheme_count: 1
schemes:
- description: Bearer token created by the endpoint "POST AccessTokenList"
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/ixon-openapi.json
  type: http
slug: ixon-authentication
source_filename: ixon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ixon-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: Bearer token created by the endpoint \"POST AccessTokenList\"\n  sources:\n  - openapi/ixon-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ixon/refs/heads/main/authentication/ixon-authentication.yml
summary_line: http · 1 scheme
tags:
- IIoT
- Industrial IoT
- Machine Connectivity
- Remote Access
---
