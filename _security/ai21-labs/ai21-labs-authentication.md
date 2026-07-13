---
api_key_in: []
api_specs:
- filename: ai21-labs-asyncapi.yml
  format: yaml
  label: AI21 Jamba Chat Completions API
  slug: chat-completions
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai21-labs/refs/heads/main/asyncapi/ai21-labs-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ai21 Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI21 Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AI21 Labs
provider_slug: ai21-labs
scheme_count: 1
schemes:
- description: Bearer API key in Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ai21-labs-openapi.yml
  type: http
slug: ai21-labs-authentication
source_filename: ai21-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ai21-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer API key in Authorization header.\n  sources:\n  - openapi/ai21-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai21-labs/refs/heads/main/authentication/ai21-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Foundation Models
- LLM
- Jamba
- Mamba
- RAG
- Agents
- Maestro
- Inference
- Enterprise AI
- Fine-Tuning
---
