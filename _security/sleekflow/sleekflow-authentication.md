---
api_key_in:
- header
api_specs:
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Conversations & Messaging API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Companies API
  slug: companies
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Lists API
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Staff & Teams API
  slug: staff-teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
- filename: sleekflow-openapi.yml
  format: yaml
  label: SleekFlow Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/openapi/sleekflow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sleekflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: SleekFlow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SleekFlow
provider_slug: sleekflow
scheme_count: 1
schemes:
- description: Platform API key issued from the SleekFlow Integrations dashboard (Admin access required).
  in: header
  name: ApiKeyAuth
  parameter: X-Sleekflow-ApiKey
  sources:
  - openapi/sleekflow-openapi.yml
  type: apiKey
slug: sleekflow-authentication
source_filename: sleekflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sleekflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Sleekflow-ApiKey\n  description: Platform API key issued from the SleekFlow Integrations dashboard (Admin access\n    required).\n  sources:\n  - openapi/sleekflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleekflow/refs/heads/main/authentication/sleekflow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Messaging
- Omnichannel
- WhatsApp
- Customer Engagement
- Social Commerce
- Automation
---
