---
api_key_in:
- header
api_specs:
- filename: codacy-account-api-openapi.yml
  format: yaml
  label: Codacy Account API
  slug: codacy-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-account-api-openapi.yml
- filename: codacy-coverage-api-openapi.yml
  format: yaml
  label: Codacy Coverage API
  slug: codacy-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-coverage-api-openapi.yml
- filename: codacy-issues-api-openapi.yml
  format: yaml
  label: Codacy Issues API
  slug: codacy-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-issues-api-openapi.yml
- filename: codacy-organizations-api-openapi.yml
  format: yaml
  label: Codacy Organizations API
  slug: codacy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-organizations-api-openapi.yml
- filename: codacy-pull-requests-api-openapi.yml
  format: yaml
  label: Codacy Pull Requests API
  slug: codacy-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-pull-requests-api-openapi.yml
- filename: codacy-quality-settings-api-openapi.yml
  format: yaml
  label: Codacy Quality Settings API
  slug: codacy-quality-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-quality-settings-api-openapi.yml
- filename: codacy-repositories-api-openapi.yml
  format: yaml
  label: Codacy Repositories API
  slug: codacy-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-repositories-api-openapi.yml
- filename: codacy-security-api-openapi.yml
  format: yaml
  label: Codacy Security API
  slug: codacy-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-security-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codacy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codacy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codacy
provider_slug: codacy
scheme_count: 1
schemes:
- description: Account API token created in your Codacy account settings.
  in: header
  name: api-token
  parameter: api-token
  sources:
  - openapi/codacy-openapi.yml
  type: apiKey
slug: codacy-authentication
source_filename: codacy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codacy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  parameter: api-token\n  description: Account API token created in your Codacy account settings.\n  sources:\n  - openapi/codacy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/authentication/codacy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Code Quality
- Static Analysis
- Security
- Code Coverage
- DevOps
---
