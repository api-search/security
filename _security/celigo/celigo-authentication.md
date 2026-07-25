---
api_key_in: []
api_specs:
- filename: celigo-webhook-listeners-asyncapi.yml
  format: yaml
  label: Celigo integrator.io Webhook Listeners
  slug: celigo-webhook-listeners
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/asyncapi/celigo-webhook-listeners-asyncapi.yml
- filename: celigo-connections-api-openapi.yml
  format: yaml
  label: Celigo Connections API
  slug: celigo-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-connections-api-openapi.yml
- filename: celigo-exports-api-openapi.yml
  format: yaml
  label: Celigo Exports API
  slug: celigo-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-exports-api-openapi.yml
- filename: celigo-flows-api-openapi.yml
  format: yaml
  label: Celigo Flows API
  slug: celigo-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-flows-api-openapi.yml
- filename: celigo-iclients-api-openapi.yml
  format: yaml
  label: Celigo iClients API
  slug: celigo-iclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-iclients-api-openapi.yml
- filename: celigo-imports-api-openapi.yml
  format: yaml
  label: Celigo Imports API
  slug: celigo-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-imports-api-openapi.yml
- filename: celigo-integrations-api-openapi.yml
  format: yaml
  label: Celigo Integrations API
  slug: celigo-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-integrations-api-openapi.yml
- filename: celigo-jobs-api-openapi.yml
  format: yaml
  label: Celigo Jobs API
  slug: celigo-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-jobs-api-openapi.yml
- filename: celigo-licenses-api-openapi.yml
  format: yaml
  label: Celigo Licenses API
  slug: celigo-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-licenses-api-openapi.yml
- filename: celigo-state-api-openapi.yml
  format: yaml
  label: Celigo State API
  slug: celigo-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/openapi/celigo-state-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Celigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celigo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Celigo
provider_slug: celigo
scheme_count: 1
schemes:
- description: 'Personal API token or OAuth 2.0 bearer token. Rate-limited using a

    token-bucket of 1000 tokens, refilled at 300 tokens per second.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/celigo-openapi.yml
  type: http
slug: celigo-authentication
source_filename: celigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/celigo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Personal API token or OAuth 2.0 bearer token. Rate-limited using a\n    token-bucket of 1000 tokens, refilled at 300 tokens per second.\n  sources:\n  - openapi/celigo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/authentication/celigo-authentication.yml
summary_line: http · 1 scheme
tags:
- API Management
- Automation
- Data Integration
- Integration
- iPaaS
- Workflow
---
