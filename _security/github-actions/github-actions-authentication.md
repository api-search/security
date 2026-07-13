---
api_key_in: []
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Actions API
  slug: github-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Github Actions Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitHub Actions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitHub Actions
provider_slug: github-actions
scheme_count: 1
schemes:
- description: GitHub personal access token or OAuth token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/github-actions-openapi.yml
  type: http
slug: github-actions-authentication
source_filename: github-actions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/github-actions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: GitHub personal access token or OAuth token\n  sources:\n  - openapi/github-actions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/authentication/github-actions-authentication.yml
summary_line: http · 1 scheme
tags: []
---
