---
api_key_in:
- header
api_specs:
- filename: arc-prize-foundation-arc-agi-3-openapi.yaml
  format: yaml
  label: ARC-AGI-3 REST API
  slug: arc-agi-3-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/openapi/arc-prize-foundation-arc-agi-3-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arc Prize Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arc Prize Foundation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arc Prize Foundation
provider_slug: arc-prize-foundation
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/arc-prize-foundation-arc-agi-3-openapi.yaml
  type: apiKey
slug: arc-prize-foundation-authentication
source_filename: arc-prize-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arc-prize-foundation-arc-agi-3-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/arc-prize-foundation-arc-agi-3-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arc-prize-foundation/refs/heads/main/authentication/arc-prize-foundation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- AGI
- Benchmarks
- Agents
- Reasoning
- Machine Learning
- Nonprofit
---
