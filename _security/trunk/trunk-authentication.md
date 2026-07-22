---
api_key_in:
- header
api_specs:
- filename: trunk-openapi.yml
  format: yaml
  label: Trunk Flaky Tests API
  slug: flaky-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/openapi/trunk-openapi.yml
- filename: trunk-openapi.yml
  format: yaml
  label: Trunk Merge Queue API
  slug: merge-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/openapi/trunk-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trunk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trunk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trunk
provider_slug: trunk
scheme_count: 1
schemes:
- description: Organization API token from Settings > Organization > General > API.
  in: header
  name: ApiKeyAuth
  parameter: x-api-token
  sources:
  - openapi/trunk-openapi.yml
  type: apiKey
slug: trunk-authentication
source_filename: trunk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/trunk-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  description: Organization API token from Settings > Organization > General > API.\n  sources:\n  - openapi/trunk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trunk/refs/heads/main/authentication/trunk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Developer Tools
- CI/CD
- Code Quality
- Flaky Tests
- Merge Queue
- Test Analytics
- Static Analysis
- Webhooks
---
