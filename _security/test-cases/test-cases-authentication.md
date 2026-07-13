---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Test Cases Authentication
name_suffix: Authentication
oauth_flows: []
overview: Test Cases secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Test Cases
provider_slug: test-cases
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/test-cases-openapi.yml
  type: apiKey
slug: test-cases-authentication
source_filename: test-cases-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/test-cases-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/test-cases-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-cases/refs/heads/main/authentication/test-cases-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Testing
- Automation
- Quality Assurance
- Software Development
- Software Testing
- Testing
---
