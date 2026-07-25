---
api_key_in:
- header
api_specs:
- filename: faros-account-api-openapi.yml
  format: yaml
  label: Faros AI Account API
  slug: faros-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-account-api-openapi.yml
- filename: faros-events-api-openapi.yml
  format: yaml
  label: Faros AI Events API
  slug: faros-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-events-api-openapi.yml
- filename: faros-graphql-api-openapi.yml
  format: yaml
  label: Faros AI GraphQL API
  slug: faros-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-graphql-api-openapi.yml
- filename: faros-graphs-api-openapi.yml
  format: yaml
  label: Faros AI Graphs API
  slug: faros-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-graphs-api-openapi.yml
- filename: faros-ingestion-api-openapi.yml
  format: yaml
  label: Faros AI Ingestion API
  slug: faros-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-ingestion-api-openapi.yml
- filename: faros-webhooks-api-openapi.yml
  format: yaml
  label: Faros AI Webhooks API
  slug: faros-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/openapi/faros-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Faros Authentication
name_suffix: Authentication
oauth_flows: []
overview: Faros AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Faros AI
provider_slug: faros
scheme_count: 1
schemes:
- description: Faros API key created in the Faros application under Settings -> API Keys. Passed directly in the Authorization header.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/faros-openapi.yml
  type: apiKey
slug: faros-authentication
source_filename: faros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/faros-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Faros API key created in the Faros application under Settings -> API Keys. Passed\n    directly in the Authorization header.\n  sources:\n  - openapi/faros-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faros/refs/heads/main/authentication/faros-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Engineering Operations
- Software Engineering Intelligence
- SEI
- DORA Metrics
- Developer Productivity
- Data Ingestion
---
