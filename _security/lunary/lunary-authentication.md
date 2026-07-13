---
api_key_in: []
api_specs:
- filename: lunary-openapi.yml
  format: yaml
  label: Lunary API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lunary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunary secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lunary
provider_slug: lunary
scheme_count: 1
schemes:
- bearerFormat: Lunary project private API key (UUID)
  name: ProjectPrivateApiKeyAuth
  scheme: bearer
  sources:
  - openapi/lunary-openapi.yml
  type: http
slug: lunary-authentication
source_filename: lunary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lunary-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ProjectPrivateApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Lunary project private API key (UUID)\n  sources:\n  - openapi/lunary-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/authentication/lunary-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Evaluation
- Observability
- Open Source
- LLM
- Tracing
- Prompts
---
