---
api_key_in: []
api_specs:
- filename: test-ai-opentestdata-openapi.yaml
  format: yaml
  label: OpenTestData API
  slug: opentestdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-ai/refs/heads/main/openapi/test-ai-opentestdata-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Test Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: test.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: test.ai
provider_slug: test-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: jwt
  scheme: bearer
  sources:
  - openapi/test-ai-opentestdata-openapi.yaml
  type: http
slug: test-ai-authentication
source_filename: test-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: openapi/test-ai-opentestdata-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/test-ai-opentestdata-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-ai/refs/heads/main/authentication/test-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Testing
- Test Automation
- Quality Assurance
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Selenium
- Appium
- Developer Tools
- gRPC
- Defunct
---
