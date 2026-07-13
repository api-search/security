---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Thoughtly API
  slug: thoughtly-api
  spec_type: OpenAPI
  url: https://docs.thoughtly.com/api-reference/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Thoughtly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thoughtly secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thoughtly
provider_slug: thoughtly
scheme_count: 2
schemes:
- description: API token from Thoughtly Developer Settings.
  in: header
  name: ApiKeyAuth
  parameter: x-api-token
  sources:
  - openapi/thoughtly-api-openapi.yml
  type: apiKey
- description: Team identifier from Thoughtly Developer Settings.
  in: header
  name: TeamIdAuth
  parameter: team_id
  sources:
  - openapi/thoughtly-api-openapi.yml
  type: apiKey
slug: thoughtly-authentication
source_filename: thoughtly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thoughtly-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  description: API token from Thoughtly Developer Settings.\n  sources:\n  - openapi/thoughtly-api-openapi.yml\n- name: TeamIdAuth\n  type: apiKey\n  in: header\n  parameter: team_id\n  description: Team identifier from Thoughtly Developer Settings.\n  sources:\n  - openapi/thoughtly-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thoughtly/refs/heads/main/authentication/thoughtly-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Voice AI
- Chat AI
- Conversational AI
- AI Agents
- Outbound Calling
- Inbound Calling
- Lead Conversion
- SMS
- WhatsApp
- CRM
- Telephony
---
