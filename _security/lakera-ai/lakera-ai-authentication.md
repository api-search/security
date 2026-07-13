---
api_key_in: []
api_specs:
- filename: lakera-guard-api-openapi.yml
  format: yaml
  label: Lakera Guard API
  slug: lakera-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/openapi/lakera-guard-api-openapi.yml
- filename: lakera-platform-api-openapi.yml
  format: yaml
  label: Lakera Platform API
  slug: lakera-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/openapi/lakera-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lakera Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lakera secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lakera
provider_slug: lakera-ai
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'Lakera Guard SaaS API key issued from the Lakera platform. Pass as

    `Authorization: Bearer $LAKERA_GUARD_API_KEY`. Self-hosted deployments

    may run without authentication.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lakera-guard-api-openapi.yml
  - openapi/lakera-platform-api-openapi.yml
  type: http
slug: lakera-ai-authentication
source_filename: lakera-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lakera-guard-api-openapi.yml, openapi/lakera-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: |-\n    Lakera Guard SaaS API key issued from the Lakera platform. Pass as\n    `Authorization: Bearer $LAKERA_GUARD_API_KEY`. Self-hosted deployments\n    may run without authentication.\n  sources:\n  - openapi/lakera-guard-api-openapi.yml\n  - openapi/lakera-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakera-ai/refs/heads/main/authentication/lakera-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Security
- Artificial Intelligence
- Generative AI
- LLM Security
- Prompt Injection
- AI Guardrails
- AI Red Teaming
- Data Loss Prevention
- Content Moderation
- Check Point
---
