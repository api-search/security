---
api_key_in:
- header
api_specs:
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty CLI
  slug: qlty-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty Coverage Upload
  slug: qlty-coverage-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty Cloud API
  slug: qlty-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qlty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qlty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qlty
provider_slug: qlty
scheme_count: 1
schemes:
- description: Per-project coverage token, supplied as the QLTY_COVERAGE_TOKEN environment variable to `qlty coverage publish`. Documented as a CLI environment variable, not a documented public REST API header.
  in: header
  name: coverageToken
  parameter: QLTY_COVERAGE_TOKEN
  sources:
  - openapi/qlty-openapi.yml
  type: apiKey
slug: qlty-authentication
source_filename: qlty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qlty-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: coverageToken\n  type: apiKey\n  in: header\n  parameter: QLTY_COVERAGE_TOKEN\n  description: Per-project coverage token, supplied as the QLTY_COVERAGE_TOKEN environment variable\n    to `qlty coverage publish`. Documented as a CLI environment variable, not a documented public\n    REST API header.\n  sources:\n  - openapi/qlty-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/authentication/qlty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Code Quality
- Code Coverage
- Static Analysis
- Linting
- Developer Tools
---
