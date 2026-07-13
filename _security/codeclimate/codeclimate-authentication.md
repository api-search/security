---
api_key_in:
- header
api_specs:
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Repos API
  slug: repos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Test Coverage API
  slug: test-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Snapshots API
  slug: snapshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Velocity API
  slug: velocity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codeclimate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Code Climate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Code Climate
provider_slug: codeclimate
scheme_count: 1
schemes:
- description: 'Personal access token passed as `Authorization: Token token={TOKEN}`.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/codeclimate-openapi.yml
  type: apiKey
slug: codeclimate-authentication
source_filename: codeclimate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codeclimate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Personal access token passed as `Authorization: Token token={TOKEN}`.'\n  sources:\n  - openapi/codeclimate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/authentication/codeclimate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Code Quality
- Static Analysis
- Test Coverage
- Engineering Analytics
- DevOps
---
