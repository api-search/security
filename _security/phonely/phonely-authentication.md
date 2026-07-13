---
api_key_in:
- header
api_specs:
- filename: phonely-agents-api-openapi.yml
  format: yaml
  label: Phonely Agents API
  slug: phonely-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/openapi/phonely-agents-api-openapi.yml
- filename: phonely-webhooks-asyncapi.yml
  format: yaml
  label: Phonely Webhooks API
  slug: phonely-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/asyncapi/phonely-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phonely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phonely secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phonely
provider_slug: phonely
scheme_count: 1
schemes:
- description: API key issued from the Phonely app. Send the raw key value as the header.
  in: header
  name: ApiKeyAuth
  parameter: X-Authorization
  sources:
  - openapi/phonely-agents-api-openapi.yml
  type: apiKey
slug: phonely-authentication
source_filename: phonely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/phonely-agents-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Authorization\n  description: API key issued from the Phonely app. Send the raw key value as the header.\n  sources:\n  - openapi/phonely-agents-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/authentication/phonely-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Artificial Intelligence
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Phone
- Call Center
- Contact Center
- SMS
- Webhooks
- Workflow Automation
- Scheduling
- CRM
---
