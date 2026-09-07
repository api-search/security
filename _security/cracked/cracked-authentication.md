---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Cracked API
  slug: cracked-api
  spec_type: OpenAPI
  url: https://cracked.ai/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cracked Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cracked API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cracked API
provider_slug: cracked
scheme_count: 1
schemes:
- description: ck_live_ API key or OAuth access token
  name: bearer
  scheme: bearer
  sources:
  - openapi/cracked-openapi.json
  - openapi/cracked-openapi.yaml
  type: http
slug: cracked-authentication
source_filename: cracked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/cracked-openapi.json, openapi/cracked-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: ck_live_ API key or OAuth access token\n  sources:\n  - openapi/cracked-openapi.json\n  - openapi/cracked-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/authentication/cracked-authentication.yml
summary_line: http · 1 scheme
tags:
- ai agents
- agent tools
- mcp
- tool router
- API aggregator
- web search
- web scraping
- data enrichment
- llms.txt
- agent skills
- pay-per-call
- ai-agents
- agent-tools
- tool-router
- aggregator
- web-search
- web-scraping
- data-enrichment
- lead-generation
- ai-models
- developer-tools
- AI agents
- MCP
- lead gen
- SEO
- social media data
- ecommerce
- finance
- weather
- AI models
---
