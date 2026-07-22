---
api_key_in:
- header
api_specs:
- filename: signadot-openapi-original.yml
  format: yaml
  label: Signadot API
  slug: signadot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signadot/refs/heads/main/openapi/signadot-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signadot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signadot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Signadot
provider_slug: signadot
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: signadot-api-key
  sources:
  - openapi/signadot-openapi-original.yml
  type: apiKey
slug: signadot-authentication
source_filename: signadot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/signadot-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: signadot-api-key\n  sources:\n  - openapi/signadot-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signadot/refs/heads/main/authentication/signadot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- Kubernetes
- Testing
- Ephemeral Environments
- Microservices
- Preview Environments
- Agentic Development
- Continuous Integration
- Developer Experience
---
