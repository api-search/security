---
api_key_in:
- header
api_specs:
- filename: yonsei-pure.yaml
  format: yaml
  label: Yonsei Research Information Portal (Elsevier Pure)
  slug: pure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yonsei/refs/heads/main/openapi/yonsei-pure.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Yonsei Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yonsei University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yonsei University
provider_slug: yonsei
scheme_count: 1
schemes:
- description: Security mechanism for the API
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/yonsei-pure.yaml
  type: apiKey
slug: yonsei-authentication
source_filename: yonsei-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yonsei-pure.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Security mechanism for the API\n  sources:\n  - openapi/yonsei-pure.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yonsei/refs/heads/main/authentication/yonsei-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Library
- Repository
- South Korea
- Seoul
---
