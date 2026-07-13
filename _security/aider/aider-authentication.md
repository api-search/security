---
api_key_in:
- header
api_specs:
- filename: aider-cli-openapi.yml
  format: yaml
  label: Aider CLI
  slug: cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-cli-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aider Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aider secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aider
provider_slug: aider
scheme_count: 1
schemes:
- description: Placeholder for documentation purposes. Aider does not authenticate with an "aider API"; it reads the relevant upstream provider key (ANTHROPIC_API_KEY, OPENAI_API_KEY, etc.) from the local environment and passes it to the chosen LLM provider directly.
  in: header
  name: LLMProviderKey
  parameter: X-Provider-API-Key
  sources:
  - openapi/aider-cli-openapi.yml
  type: apiKey
slug: aider-authentication
source_filename: aider-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aider-cli-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LLMProviderKey\n  type: apiKey\n  in: header\n  parameter: X-Provider-API-Key\n  description: Placeholder for documentation purposes. Aider does not authenticate with an \"aider\n    API\"; it reads the relevant upstream provider key (ANTHROPIC_API_KEY, OPENAI_API_KEY, etc.)\n    from the local environment and passes it to the chosen LLM provider directly.\n  sources:\n  - openapi/aider-cli-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/authentication/aider-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- AI Pair Programming
- Developer Tools
- CLI
- Command Line
- Coding Assistant
- Code Generation
- Open Source
- Python
- Apache 2.0
- LLM
- Git
- BYO LLM
- Terminal
- Polyglot
- Tree Sitter
- Repository Map
- Pair Programming
---
