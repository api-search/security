---
api_key_in: []
api_specs:
- filename: relace-openapi-original.json
  format: json
  label: Relace API
  slug: relace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relace/refs/heads/main/openapi/relace-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Relace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Relace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Relace
provider_slug: relace
scheme_count: 1
schemes:
- description: Relace API key Authorization header using the Bearer scheme.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/relace-openapi-original.json
  type: http
slug: relace-authentication
source_filename: relace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/relace-openapi-original.json\ndocs: https://docs.relace.ai/api-reference/introduction\nkey_format: rlc-<32-char>\nobtain: https://app.relace.ai/settings/api-keys\nscoped_tokens: >-\n  Repo Tokens are scoped API keys created per repository for narrower access.\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Relace API key Authorization header using the Bearer scheme.\n  sources:\n  - openapi/relace-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relace/refs/heads/main/authentication/relace-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Coding Agents
- Code Generation
- Developer Tools
- Machine Learning
- Code Search
- LLM
---
