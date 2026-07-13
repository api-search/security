---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare Queues API
  slug: cloudflare-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/main/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudflare Queues Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudflare Queues secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloudflare Queues
provider_slug: cloudflare-queues
scheme_count: 3
schemes:
- description: Cloudflare API Token (Bearer)
  name: api_token
  scheme: bearer
  sources:
  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml
  type: http
- description: Cloudflare account email address
  in: header
  name: api_email
  parameter: X-Auth-Email
  sources:
  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml
  type: apiKey
- description: Cloudflare Global API Key
  in: header
  name: api_key
  parameter: X-Auth-Key
  sources:
  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml
  type: apiKey
slug: cloudflare-queues-authentication
source_filename: cloudflare-queues-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  description: Cloudflare API Token (Bearer)\n  sources:\n  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml\n- name: api_email\n  type: apiKey\n  in: header\n  parameter: X-Auth-Email\n  description: Cloudflare account email address\n  sources:\n  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  description: Cloudflare Global API Key\n  sources:\n  - openapi/cloudflare-queues-cloudflare-queues-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-queues/refs/heads/main/authentication/cloudflare-queues-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Messaging
- Message Queue
- Serverless
- Workers
- Cloudflare
- Async
- Dead Letter Queue
- Event Driven
---
