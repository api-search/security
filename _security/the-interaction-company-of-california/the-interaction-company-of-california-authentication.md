---
api_key_in: []
api_specs:
- filename: the-interaction-company-of-california-poke-openapi.yml
  format: yaml
  label: Poke API
  slug: poke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-interaction-company-of-california/refs/heads/main/openapi/the-interaction-company-of-california-poke-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: The Interaction Company Of California Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Interaction Company Of California secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Interaction Company Of California
provider_slug: the-interaction-company-of-california
scheme_count: 1
schemes:
- description: 'V2 API key generated in Kitchen, sent as `Authorization: Bearer YOUR_API_KEY`. Legacy `pk_`-prefixed V1 keys work only with the deprecated inbound-sms webhook.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/the-interaction-company-of-california-poke-openapi.yml
  type: http
slug: the-interaction-company-of-california-authentication
source_filename: the-interaction-company-of-california-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/the-interaction-company-of-california-poke-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'V2 API key generated in Kitchen, sent as `Authorization: Bearer YOUR_API_KEY`.\n    Legacy `pk_`-prefixed V1 keys work only with the deprecated inbound-sms webhook.'\n  sources:\n  - openapi/the-interaction-company-of-california-poke-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-interaction-company-of-california/refs/heads/main/authentication/the-interaction-company-of-california-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Assistant
- Artificial Intelligence
- Agents
- Messaging
- Model Context Protocol
- MCP
- Productivity
- Automation
- Conversational AI
---
