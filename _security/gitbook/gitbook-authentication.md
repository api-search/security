---
api_key_in: []
api_specs:
- filename: gitbook-gitbook-api-openapi.yml
  format: yaml
  label: GitBook
  slug: gitbook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-gitbook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitbook Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitBook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitBook
provider_slug: gitbook
scheme_count: 1
schemes:
- bearerFormat: token
  description: API access token. Generate one from the Developer settings of your GitBook user account.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gitbook-gitbook-api-openapi.yml
  type: http
slug: gitbook-authentication
source_filename: gitbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitbook-gitbook-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: API access token. Generate one from the Developer settings of your GitBook user\n    account.\n  sources:\n  - openapi/gitbook-gitbook-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/authentication/gitbook-authentication.yml
summary_line: http · 1 scheme
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
---
