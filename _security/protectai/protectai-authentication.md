---
api_key_in: []
api_specs:
- filename: protectai-openapi.yml
  format: yaml
  label: LLM Guard (Scanners)
  slug: llm-guard-scanners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protectai/refs/heads/main/openapi/protectai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Protectai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Protect AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Protect AI
provider_slug: protectai
scheme_count: 1
schemes:
- description: Optional bearer token authentication, enabled per deployment via the llm-guard-api configuration. Deployments may also run without auth.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/protectai-openapi.yml
  type: http
slug: protectai-authentication
source_filename: protectai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/protectai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional bearer token authentication, enabled per deployment via the llm-guard-api\n    configuration. Deployments may also run without auth.\n  sources:\n  - openapi/protectai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protectai/refs/heads/main/authentication/protectai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- ML
- Security
- LLM
- Guardrails
---
