---
api_key_in:
- cookie
- header
api_specs:
- filename: store
  format: yaml
  label: Medusa Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://docs.medusajs.com/api/download/store
- filename: admin
  format: yaml
  label: Medusa Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://docs.medusajs.com/api/download/admin
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Medusa Js Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medusa secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medusa
provider_slug: medusa-js
scheme_count: 3
schemes:
- description: Publishable API key that scopes requests to one or more sales channels.
  in: header
  name: publishableApiKey
  parameter: x-publishable-api-key
  sources:
  - openapi/medusa-js-openapi.yml
  type: apiKey
- description: JWT bearer token obtained via /auth/customer/{auth_provider}.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/medusa-js-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: connect.sid
  sources:
  - openapi/medusa-js-openapi.yml
  type: apiKey
slug: medusa-js-authentication
source_filename: medusa-js-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medusa-js-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: publishableApiKey\n  type: apiKey\n  in: header\n  parameter: x-publishable-api-key\n  description: Publishable API key that scopes requests to one or more sales channels.\n  sources:\n  - openapi/medusa-js-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: JWT bearer token obtained via /auth/customer/{auth_provider}.\n  sources:\n  - openapi/medusa-js-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: connect.sid\n  sources:\n  - openapi/medusa-js-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/authentication/medusa-js-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Commerce
- Headless
- eCommerce
- Open Source
- Node.js
- TypeScript
- Framework
- Modules
- Workflows
- MCP
---
