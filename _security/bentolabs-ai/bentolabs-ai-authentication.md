---
api_key_in:
- env
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bentolabs Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bentolabs AI secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bentolabs AI
provider_slug: bentolabs-ai
scheme_count: 2
schemes:
- description: Publishable ingest API key used by the SDK/exporter to ship OpenTelemetry traces to the BentoLabs ingest API. Keys begin with the `bl_pk_` prefix and the SDK validates the prefix locally before any network request.
  env_var: BENTOLABS_API_KEY
  init: bento.init(api_key="bl_pk_...")
  key_prefix: bl_pk_
  name: BentoLabsApiKey
  sources:
  - docs
  type: apiKey
- description: The `bentolabs` CLI authenticates the human user via `bentolabs auth login` (personal credentials, full dashboard parity) rather than an API key. API keys are managed per workspace (see `bentolabs api-keys`).
  name: BentoLabsUserAuth
  sources:
  - docs
  type: interactive
slug: bentolabs-ai-authentication
source_filename: bentolabs-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.bentolabs.ai/python/installation + https://docs.bentolabs.ai/python/configuration\ndocs: https://docs.bentolabs.ai/quickstart\nsummary:\n  types: [apiKey]\n  api_key_in: [env, header]\n  oauth2_flows: []\nschemes:\n- name: BentoLabsApiKey\n  type: apiKey\n  description: >-\n    Publishable ingest API key used by the SDK/exporter to ship OpenTelemetry\n    traces to the BentoLabs ingest API. Keys begin with the `bl_pk_` prefix and\n    the SDK validates the prefix locally before any network request.\n  key_prefix: bl_pk_\n  env_var: BENTOLABS_API_KEY\n  init: bento.init(api_key=\"bl_pk_...\")\n  sources: [docs]\n- name: BentoLabsUserAuth\n  type: interactive\n  description: >-\n    The `bentolabs` CLI authenticates the human user via `bentolabs auth login`\n    (personal credentials, full dashboard parity) rather than an API key. API\n    keys are managed per workspace (see `bentolabs api-keys`).\n  sources: [docs]\n\
  notes: >-\n  No published product OpenAPI was found (the docs `api-reference/openapi.json`\n  is the Mintlify Plant Store placeholder), so schemes are captured from the\n  documentation rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bentolabs-ai/refs/heads/main/authentication/bentolabs-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI Agents
- Observability
- OpenTelemetry
- Tracing
- LLM Monitoring
- Evaluation
- Agent Infrastructure
- Developer Tools
---
