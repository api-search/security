---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Postman Collections API
  slug: postman-collections-api
  spec_type: OpenAPI
  url: https://www.postman.com/postman/postman-public-workspace/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Test Suites Authentication
name_suffix: Authentication
oauth_flows: []
overview: Test Suites secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Test Suites
provider_slug: test-suites
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/test-suites-openapi.yml
  type: apiKey
slug: test-suites-authentication
source_filename: test-suites-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/test-suites-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/test-suites-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-suites/refs/heads/main/authentication/test-suites-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Testing
- Collections
- Quality Assurance
- Software Development
- Test Management
- Testing
---
