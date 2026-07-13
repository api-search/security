---
api_key_in: []
api_specs:
- filename: crewai-amp-rest-api-openapi.yml
  format: yaml
  label: CrewAI AMP REST API
  slug: crewai-amp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/openapi/crewai-amp-rest-api-openapi.yml
- filename: crewai-amp-webhooks-asyncapi.yml
  format: yaml
  label: CrewAI AMP Webhook Streaming
  slug: crewai-amp-webhook-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/asyncapi/crewai-amp-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Crewai Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrewAI Cloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CrewAI Cloud
provider_slug: crewai-cloud
scheme_count: 1
schemes:
- bearerFormat: opaque
  description: 'Bearer token from the AMP dashboard Status tab. Use either an organization-level

    Bearer Token (full crew operations) or a User Bearer Token (user-scoped access).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/crewai-amp-rest-api-openapi.yml
  type: http
slug: crewai-cloud-authentication
source_filename: crewai-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crewai-amp-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: |-\n    Bearer token from the AMP dashboard Status tab. Use either an organization-level\n    Bearer Token (full crew operations) or a User Bearer Token (user-scoped access).\n  sources:\n  - openapi/crewai-amp-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crewai-cloud/refs/heads/main/authentication/crewai-cloud-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- AI Agent Platform
- Agent Orchestration
- Multi-Agent Systems
- Agent Management Platform
- Managed Agents
- Automations
- Observability
- Human In The Loop
---
