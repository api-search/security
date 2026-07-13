---
api_key_in: []
api_specs:
- filename: cleanlab-openapi.yml
  format: yaml
  label: Trustworthy Language Model (TLM)
  slug: trustworthy-language-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
- filename: cleanlab-openapi.yml
  format: yaml
  label: Cleanlab Studio
  slug: cleanlab-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
- filename: cleanlab-openapi.yml
  format: yaml
  label: Codex
  slug: codex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/openapi/cleanlab-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cleanlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleanlab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cleanlab
provider_slug: cleanlab
scheme_count: 1
schemes:
- description: Cleanlab API key (TLM / Studio) or Codex project access key, supplied as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cleanlab-openapi.yml
  type: http
slug: cleanlab-authentication
source_filename: cleanlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cleanlab-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Cleanlab API key (TLM / Studio) or Codex project access key, supplied as a Bearer\n    token in the Authorization header.\n  sources:\n  - openapi/cleanlab-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanlab/refs/heads/main/authentication/cleanlab-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Trustworthiness
- Data Quality
- Guardrails
---
