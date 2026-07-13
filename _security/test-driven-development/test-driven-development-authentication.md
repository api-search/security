---
api_key_in: []
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Actions API
  slug: github-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: openapi.json
  format: json
  label: CircleCI API
  slug: circleci-api
  spec_type: OpenAPI
  url: https://circleci.com/api/v2/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Test Driven Development Authentication
name_suffix: Authentication
oauth_flows: []
overview: Test-Driven Development secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Test-Driven Development
provider_slug: test-driven-development
scheme_count: 1
schemes:
- bearerFormat: GitHub token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/test-driven-development-openapi.yml
  type: http
slug: test-driven-development-authentication
source_filename: test-driven-development-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/test-driven-development-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: GitHub token\n  sources:\n  - openapi/test-driven-development-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-driven-development/refs/heads/main/authentication/test-driven-development-authentication.yml
summary_line: http · 1 scheme
tags:
- Agile
- Best Practices
- Continuous Integration
- Extreme Programming
- Methodology
- Software Development
- Testing
---
