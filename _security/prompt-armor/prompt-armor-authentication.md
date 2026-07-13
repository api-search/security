---
api_key_in:
- header
api_specs:
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Content Check API
  slug: prompt-armor-content-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Analyze API
  slug: prompt-armor-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Session Monitoring API
  slug: prompt-armor-session-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prompt Armor Authentication
name_suffix: Authentication
oauth_flows: []
overview: PromptArmor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PromptArmor
provider_slug: prompt-armor
scheme_count: 1
schemes:
- description: PromptArmor API key passed in the Api-Key request header.
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/prompt-armor-openapi.yml
  type: apiKey
slug: prompt-armor-authentication
source_filename: prompt-armor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prompt-armor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: PromptArmor API key passed in the Api-Key request header.\n  sources:\n  - openapi/prompt-armor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/authentication/prompt-armor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- LLM
- Security
- Prompt Injection
- Threat Detection
---
