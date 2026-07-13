---
api_key_in:
- header
api_specs:
- filename: regal-events-api-openapi.yml
  format: yaml
  label: Regal Events API
  slug: regal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-events-api-openapi.yml
- filename: regal-branded-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Branded Phone Numbers API
  slug: regal-branded-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-branded-phone-numbers-api-openapi.yml
- filename: regal-management-api-openapi.yml
  format: yaml
  label: Regal Management API
  slug: regal-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-management-api-openapi.yml
- filename: regal-messages-api-openapi.yml
  format: yaml
  label: Regal Messages API
  slug: regal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-messages-api-openapi.yml
- filename: regal-reporting-webhooks-asyncapi.yml
  format: yaml
  label: Regal Reporting Webhooks
  slug: regal-reporting-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/asyncapi/regal-reporting-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Regal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Regal
provider_slug: regal-ai
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/regal-branded-phone-numbers-api-openapi.yml
  - openapi/regal-events-api-openapi.yml
  - openapi/regal-management-api-openapi.yml
  - openapi/regal-messages-api-openapi.yml
  type: apiKey
slug: regal-ai-authentication
source_filename: regal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regal-branded-phone-numbers-api-openapi.yml, openapi/regal-events-api-openapi.yml,\n  openapi/regal-management-api-openapi.yml, openapi/regal-messages-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/regal-branded-phone-numbers-api-openapi.yml\n  - openapi/regal-events-api-openapi.yml\n  - openapi/regal-management-api-openapi.yml\n  - openapi/regal-messages-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/authentication/regal-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- AI Agents
- Voice AI
- Contact Center
- Outbound Calling
- Inbound Calling
- Phone Agents
- SMS
- Chat
- WebRTC
- Conversation Intelligence
- Journey Orchestration
- Branded Caller ID
- CCaaS
- CPaaS
- Sales Dialer
- Customer Engagement
---
