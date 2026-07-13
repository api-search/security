---
api_key_in:
- header
api_specs:
- filename: 72a32ca1-f3a2-4a5e-91f2-token
  format: yaml
  label: Postman API
  slug: postman-api
  spec_type: OpenAPI
  url: https://www.postman.com/postman/postman-public-workspace/api/72a32ca1-f3a2-4a5e-91f2-token
- filename: openapi.yaml
  format: yaml
  label: k6 Performance Testing
  slug: k6-performance-testing
  spec_type: OpenAPI
  url: https://grafana.com/docs/k6/latest/misc/k6-rest-api/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Test Scripts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Test Scripts secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Test Scripts
provider_slug: test-scripts
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/test-scripts-openapi.yml
  type: apiKey
slug: test-scripts-authentication
source_filename: test-scripts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/test-scripts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/test-scripts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-scripts/refs/heads/main/authentication/test-scripts-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- CI/CD
- Contract Testing
- Quality Assurance
- Software Development
- Testing
---
