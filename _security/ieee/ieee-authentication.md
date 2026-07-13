---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ieee Authentication
name_suffix: Authentication
oauth_flows: []
overview: IEEE Xplore secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IEEE Xplore
provider_slug: ieee
scheme_count: 1
schemes:
- description: API key obtained by registering at https://developer.ieee.org/member/register. Must be appended to every request as the apikey query parameter.
  in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: ieee-authentication
source_filename: ieee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key obtained by registering at https://developer.ieee.org/member/register.\n    Must be appended to every request as the apikey query parameter.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ieee/refs/heads/main/authentication/ieee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Science And Math
- Scholarly Publishing
- Engineering
- Computer Science
- Standards
- Research
- Academic
- Technology
---
