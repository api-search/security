---
api_key_in:
- header
api_specs:
- filename: rainforest-qa-openapi-original.yml
  format: yaml
  label: Rainforest API
  slug: rainforest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rainforest Qa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainforest QA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rainforest QA
provider_slug: rainforest-qa
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: CLIENT_TOKEN
  sources:
  - openapi/rainforest-qa-openapi-original.yml
  type: apiKey
slug: rainforest-qa-authentication
source_filename: rainforest-qa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/rainforest-qa-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: CLIENT_TOKEN\n  sources:\n  - openapi/rainforest-qa-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/authentication/rainforest-qa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Testing
- QA
- Test Automation
- Software Testing
- CI/CD
- Quality Assurance
- Crowdsourced Testing
- No-Code
- Developer Tools
---
