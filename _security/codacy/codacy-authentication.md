---
api_key_in:
- header
api_specs:
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Organizations API
  slug: organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Repositories API
  slug: repositories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Pull Requests API
  slug: pull-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Coverage API
  slug: coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
- filename: codacy-openapi.yml
  format: yaml
  label: Codacy Security API
  slug: security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codacy/refs/heads/main/openapi/codacy-openapi.yml
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
