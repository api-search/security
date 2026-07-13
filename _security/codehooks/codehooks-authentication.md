---
api_key_in:
- header
api_specs:
- filename: codehooks-database-rest-api-openapi.yml
  format: yaml
  label: Codehooks Database REST API
  slug: codehooks-database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/openapi/codehooks-database-rest-api-openapi.yml
- filename: codehooks-events-asyncapi.yml
  format: yaml
  label: Codehooks Events (AsyncAPI)
  slug: codehooks-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/asyncapi/codehooks-events-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Codehooks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codehooks secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Codehooks
provider_slug: codehooks
scheme_count: 2
schemes:
- description: API key for authentication. Obtain from the Codehooks.io dashboard or CLI.
  in: header
  name: apiKey
  parameter: x-apikey
  sources:
  - openapi/codehooks-database-rest-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT token for authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/codehooks-database-rest-api-openapi.yml
  type: http
slug: codehooks-authentication
source_filename: codehooks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codehooks-database-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-apikey\n  description: API key for authentication. Obtain from the Codehooks.io dashboard or CLI.\n  sources:\n  - openapi/codehooks-database-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token for authentication\n  sources:\n  - openapi/codehooks-database-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/authentication/codehooks-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Backend
- Database
- Events
- Hooks
- JavaScript
- NoSQL
- Queues
- Serverless
- Webhooks
- Workers
- Workflows
---
