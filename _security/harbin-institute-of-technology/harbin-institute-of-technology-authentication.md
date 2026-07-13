---
api_key_in:
- header
api_specs:
- filename: harbin-institute-of-technology-pure.yaml
  format: yaml
  label: HIT Research Portal OAI-PMH
  slug: pure-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbin-institute-of-technology/refs/heads/main/openapi/harbin-institute-of-technology-pure.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harbin Institute Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbin Institute of Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harbin Institute of Technology
provider_slug: harbin-institute-of-technology
scheme_count: 1
schemes:
- description: Pure API key. The HIT instance requires an issued key for API access.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/harbin-institute-of-technology-pure.yaml
  type: apiKey
slug: harbin-institute-of-technology-authentication
source_filename: harbin-institute-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harbin-institute-of-technology-pure.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Pure API key. The HIT instance requires an issued key for API access.\n  sources:\n  - openapi/harbin-institute-of-technology-pure.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbin-institute-of-technology/refs/heads/main/authentication/harbin-institute-of-technology-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Scholarly
- OAI-PMH
- China
---
