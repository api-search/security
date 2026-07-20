---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cumulus Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cumulus Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cumulus Labs
provider_slug: cumulus-labs
scheme_count: 1
schemes:
- description: 'Cumulus API key sent as `Authorization: Bearer <CUMULUS_KEY>`. The gateway is drop-in compatible with the OpenAI SDK — set base_url to https://api.cumuluslabs.io/v1 and api_key to your Cumulus key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://cumuluslabs.io/
  type: http
slug: cumulus-labs-authentication
source_filename: cumulus-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cumuluslabs.io/\ndocs: https://docs.cumuluslabs.io/getting-started/\nsummary:\n  types: [http]\n  http_scheme: bearer\n  api_key_in: [header]\n  notes: >-\n    OpenAI-compatible bearer authentication. The Cumulus API key is passed as\n    the OpenAI SDK `api_key` (read from the CUMULUS_KEY environment variable in\n    the published quickstart) and sent as an HTTP `Authorization: Bearer <key>`\n    header against the base URL https://api.cumuluslabs.io/v1. Tunnel URLs for\n    live inference servers also require the Cumulus API key.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Cumulus API key sent as `Authorization: Bearer <CUMULUS_KEY>`. The gateway\n    is drop-in compatible with the OpenAI SDK — set base_url to\n    https://api.cumuluslabs.io/v1 and api_key to your Cumulus key.\n  sources: [https://cumuluslabs.io/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumulus-labs/refs/heads/main/authentication/cumulus-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Inference
- LLM
- AI Infrastructure
- GPU
- Machine Learning
- Model Serving
- Fine-Tuning
- API Gateway
- Y Combinator
---
