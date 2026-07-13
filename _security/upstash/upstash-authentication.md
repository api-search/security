---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Upstash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upstash secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Upstash
provider_slug: upstash
scheme_count: 2
schemes:
- description: HTTP Basic auth with Upstash account email and API key.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/upstash-openapi.yml
  type: http
- description: Database-scoped bearer token issued from the Upstash console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/upstash-openapi.yml
  type: http
slug: upstash-authentication
source_filename: upstash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upstash-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with Upstash account email and API key.\n  sources:\n  - openapi/upstash-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Database-scoped bearer token issued from the Upstash console.\n  sources:\n  - openapi/upstash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstash/refs/heads/main/authentication/upstash-authentication.yml
summary_line: http · 2 schemes
tags:
- Serverless
- Redis
- Kafka
- Messaging
- Vector Database
- Edge Computing
---
