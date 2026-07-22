---
api_key_in:
- header
api_specs:
- filename: outrival-v1-openapi-original.json
  format: json
  label: OutRival API v1
  slug: outrival-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v1-openapi-original.json
- filename: outrival-v2-openapi-original.json
  format: json
  label: OutRival API v2
  slug: outrival-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v2-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Outrival Authentication
name_suffix: Authentication
oauth_flows: []
overview: OutRival secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OutRival
provider_slug: outrival
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: X-API-Key
  sources:
  - openapi/outrival-v1-openapi-original.json
  - openapi/outrival-v2-openapi-original.json
  type: apiKey
slug: outrival-authentication
source_filename: outrival-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/outrival-v1-openapi-original.json, openapi/outrival-v2-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/outrival-v1-openapi-original.json\n  - openapi/outrival-v2-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/authentication/outrival-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise Saas
- Conversational AI
- AI Agents
- Voice
- SMS
- Customer Engagement
- Chatbots
- Contact Center
- Webhooks
---
