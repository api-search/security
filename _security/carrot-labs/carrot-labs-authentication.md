---
api_key_in:
- sdk
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Carrot Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carrot Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carrot Labs
provider_slug: carrot-labs
scheme_count: 1
schemes:
- env_var: SP_API_KEY
  in: sdk
  init: sp.init(api_key="sp-...")
  key_prefix: sp-
  name: SuperPenguinApiKey
  notes: API keys are created in the dashboard at app.superpenguin.ai/proxies and are shown only once. Keys are passed to the SDK via sp.init(api_key=...) or the SP_API_KEY environment variable. Keys must be kept server-side for TypeScript/JavaScript applications. No OAuth2 or OpenID Connect surface is documented; the SuperPenguin backend does not publish an OpenAPI spec.
  provisioning: https://app.superpenguin.ai/proxies
  type: apiKey
slug: carrot-labs-authentication
source_filename: carrot-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://superpenguin.ai/docs\ndocs: https://superpenguin.ai/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - sdk\n  oauth2_flows: []\nschemes:\n- name: SuperPenguinApiKey\n  type: apiKey\n  in: sdk\n  key_prefix: \"sp-\"\n  env_var: SP_API_KEY\n  init: 'sp.init(api_key=\"sp-...\")'\n  provisioning: https://app.superpenguin.ai/proxies\n  notes: >-\n    API keys are created in the dashboard at app.superpenguin.ai/proxies and are\n    shown only once. Keys are passed to the SDK via sp.init(api_key=...) or the\n    SP_API_KEY environment variable. Keys must be kept server-side for\n    TypeScript/JavaScript applications. No OAuth2 or OpenID Connect surface is\n    documented; the SuperPenguin backend does not publish an OpenAPI spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrot-labs/refs/heads/main/authentication/carrot-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- FinOps
- AIOps
- Cost Management
- LLM
- Observability
- Developer Tools
---
