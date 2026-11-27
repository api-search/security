---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: infivoice-agents-api-openapi.yml
  format: yaml
  label: InfiVoice Agents API
  slug: infivoice-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-agents-api-openapi.yml
- filename: infivoice-analytics-api-openapi.yml
  format: yaml
  label: InfiVoice Analytics API
  slug: infivoice-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-analytics-api-openapi.yml
- filename: infivoice-calls-api-openapi.yml
  format: yaml
  label: InfiVoice Calls API
  slug: infivoice-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-calls-api-openapi.yml
- filename: infivoice-campaigns-api-openapi.yml
  format: yaml
  label: InfiVoice Campaigns API
  slug: infivoice-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-campaigns-api-openapi.yml
- filename: infivoice-contacts-api-openapi.yml
  format: yaml
  label: InfiVoice Contacts API
  slug: infivoice-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-contacts-api-openapi.yml
- filename: infivoice-credits-api-openapi.yml
  format: yaml
  label: InfiVoice Credits API
  slug: infivoice-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-credits-api-openapi.yml
- filename: infivoice-introduction-api-openapi.yml
  format: yaml
  label: InfiVoice Introduction API
  slug: infivoice-introduction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-introduction-api-openapi.yml
- filename: infivoice-webhooks-api-openapi.yml
  format: yaml
  label: InfiVoice Webhooks API
  slug: infivoice-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infivoice/openapi/infivoice-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: InfiVoice Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfiVoice secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: InfiVoice
provider_slug: infivoice
scheme_count: 2
schemes:
- description: API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/infivoice-openapi.json
  type: apiKey
- description: Bearer token (API key)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/infivoice-openapi.json
  type: http
slug: infivoice-authentication
source_filename: infivoice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/infivoice-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authentication\n  sources:\n  - openapi/infivoice-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token (API key)\n  sources:\n  - openapi/infivoice-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/infivoice/authentication/infivoice-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Voice
- Automation
- Software-as-a-Service
---
