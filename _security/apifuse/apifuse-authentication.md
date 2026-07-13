---
api_key_in:
- header
api_specs:
- filename: apifuse-api.yaml
  format: yaml
  label: Apifuse API
  slug: apifuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/openapi/apifuse-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apifuse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apifuse secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apifuse
provider_slug: apifuse
scheme_count: 1
schemes:
- description: API key for authenticating requests to the Apifuse API.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/apifuse-api.yaml
  type: apiKey
slug: apifuse-authentication
source_filename: apifuse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apifuse-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating requests to the Apifuse API.\n  sources:\n  - openapi/apifuse-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/authentication/apifuse-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
---
