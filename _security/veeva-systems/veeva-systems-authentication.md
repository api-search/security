---
api_key_in:
- header
api_specs:
- filename: veeva-systems-openapi.yml
  format: yaml
  label: Veeva Systems API
  slug: veeva-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva-systems/refs/heads/main/openapi/veeva-systems-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Veeva Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veeva Systems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veeva Systems
provider_slug: veeva-systems
scheme_count: 1
schemes:
- description: Vault Session ID returned by /auth, sent as the Authorization header.
  in: header
  name: SessionId
  parameter: Authorization
  sources:
  - openapi/veeva-systems-openapi.yml
  type: apiKey
slug: veeva-systems-authentication
source_filename: veeva-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veeva-systems-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SessionId\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Vault Session ID returned by /auth, sent as the Authorization header.\n  sources:\n  - openapi/veeva-systems-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva-systems/refs/heads/main/authentication/veeva-systems-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- SaaS
- Life Sciences
---
