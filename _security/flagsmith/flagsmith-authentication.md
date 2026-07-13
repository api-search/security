---
api_key_in:
- header
api_specs:
- filename: flagsmith-flags-api-openapi.yml
  format: yaml
  label: Flagsmith Flags API
  slug: flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-flags-api-openapi.yml
- filename: flagsmith-admin-api-openapi.yml
  format: yaml
  label: Flagsmith Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/openapi/flagsmith-admin-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flagsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: flagsmith secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: flagsmith
provider_slug: flagsmith
scheme_count: 2
schemes:
- description: A secret Organisation API Token prefixed with 'Api-Key'. For example, 'Api-Key your-token-here'. This token should never be exposed in client-side code.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/flagsmith-admin-api-openapi.yml
  type: apiKey
- description: A non-secret environment key used to identify which Flagsmith environment to evaluate flags against. This key is safe to include in client-side code.
  in: header
  name: environmentKey
  parameter: X-Environment-Key
  sources:
  - openapi/flagsmith-flags-api-openapi.yml
  type: apiKey
slug: flagsmith-authentication
source_filename: flagsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flagsmith-admin-api-openapi.yml, openapi/flagsmith-flags-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A secret Organisation API Token prefixed with 'Api-Key'. For example, 'Api-Key\n    your-token-here'. This token should never be exposed in client-side code.\n  sources:\n  - openapi/flagsmith-admin-api-openapi.yml\n- name: environmentKey\n  type: apiKey\n  in: header\n  parameter: X-Environment-Key\n  description: A non-secret environment key used to identify which Flagsmith environment to\n    evaluate flags against. This key is safe to include in client-side code.\n  sources:\n  - openapi/flagsmith-flags-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flagsmith/refs/heads/main/authentication/flagsmith-authentication.yml
summary_line: apiKey · 2 schemes
tags: []
---
