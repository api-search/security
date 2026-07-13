---
api_key_in:
- header
api_specs:
- filename: pixie-openapi.yml
  format: yaml
  label: Pixie API
  slug: pixie
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixie/refs/heads/main/openapi/pixie-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pixie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixie secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixie
provider_slug: pixie
scheme_count: 1
schemes:
- description: Pixie API key for authenticating requests. Generate an API key from the Pixie Cloud UI under Profile > API Keys.
  in: header
  name: apiKeyAuth
  parameter: pixie-api-key
  sources:
  - openapi/pixie-openapi.yml
  type: apiKey
slug: pixie-authentication
source_filename: pixie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pixie-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: pixie-api-key\n  description: Pixie API key for authenticating requests. Generate an API key from the Pixie\n    Cloud UI under Profile > API Keys.\n  sources:\n  - openapi/pixie-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixie/refs/heads/main/authentication/pixie-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- eBPF
- Kubernetes
- Monitoring
- Observability
---
