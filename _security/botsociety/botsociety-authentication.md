---
api_key_in:
- header
api_specs:
- filename: botsociety-openapi.yml
  format: yaml
  label: Botsociety API
  slug: botsociety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botsociety/refs/heads/main/openapi/botsociety-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Botsociety Authentication
name_suffix: Authentication
oauth_flows: []
overview: BotSociety secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BotSociety
provider_slug: botsociety
scheme_count: 2
schemes:
- description: The Botsociety user id, obtained from the Botsociety app.
  in: header
  name: user_id
  parameter: user_id
  sources:
  - openapi/botsociety-openapi.yml
  type: apiKey
- description: The Botsociety public API key, obtained from the Botsociety app.
  in: header
  name: api_key_public
  parameter: api_key_public
  sources:
  - openapi/botsociety-openapi.yml
  type: apiKey
slug: botsociety-authentication
source_filename: botsociety-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/botsociety-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: user_id\n  type: apiKey\n  in: header\n  parameter: user_id\n  description: The Botsociety user id, obtained from the Botsociety app.\n  sources:\n  - openapi/botsociety-openapi.yml\n- name: api_key_public\n  type: apiKey\n  in: header\n  parameter: api_key_public\n  description: The Botsociety public API key, obtained from the Botsociety app.\n  sources:\n  - openapi/botsociety-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botsociety/refs/heads/main/authentication/botsociety-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Chatbots
- Conversational AI
- Voice Assistants
- Bot Design
- Prototyping
- Developer Tools
---
