---
api_key_in:
- header
api_specs:
- filename: osmosis-agent-improvement-openapi.json
  format: json
  label: Osmosis Agent Improvement API
  slug: osmosis-agent-improvement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/openapi/osmosis-agent-improvement-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Osmosis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Osmosis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Osmosis
provider_slug: osmosis
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/osmosis-agent-improvement-openapi.json
  type: apiKey
slug: osmosis-authentication
source_filename: osmosis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/osmosis-agent-improvement-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/osmosis-agent-improvement-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/authentication/osmosis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Reinforcement Learning
- LLM
- Post-Training
- Model Training
- Agents
- Machine Learning
- Developer Tools
---
