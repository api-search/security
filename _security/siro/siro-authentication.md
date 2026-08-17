---
api_key_in:
- header
api_specs:
- filename: siro-audit-api-openapi.yml
  format: yaml
  label: Siro Audit API
  slug: siro-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-audit-api-openapi.yml
- filename: siro-core-api-openapi.yml
  format: yaml
  label: Siro Core API
  slug: siro-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-core-api-openapi.yml
- filename: siro-folders-api-openapi.yml
  format: yaml
  label: Siro Folders API
  slug: siro-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-folders-api-openapi.yml
- filename: siro-integrations-api-openapi.yml
  format: yaml
  label: Siro Integrations API
  slug: siro-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-integrations-api-openapi.yml
- filename: siro-platform-api-openapi.json
  format: json
  label: Siro Platform API
  slug: siro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/_original/siro-platform-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Siro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Siro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Siro
provider_slug: siro
scheme_count: 2
schemes:
- bearerFormat: Organization API token
  description: 'Organization integration token from Siro admin (Person icon → API Tokens). Send Authorization: Bearer <organization-api-token>. This is not the OAuth access token used with api.siro.ai user-scoped endpoints.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/siro-external-api-openapi.json
  - openapi/siro-openapi-original.json
  type: http
- description: 'OAuth access token for user-scoped requests (Authorization Code or machine-to-machine). Send header `x-siro-auth-token: <oauth-access-token>`. Not an organization API key.'
  in: header
  name: SiroAuthToken
  parameter: x-siro-auth-token
  sources:
  - openapi/siro-folders-api-openapi.json
  - openapi/siro-recordings-api-openapi.json
  type: apiKey
slug: siro-authentication
source_filename: siro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/siro-external-api-openapi.json, openapi/siro-folders-api-openapi.json, openapi/siro-openapi-original.json,\n  openapi/siro-recordings-api-openapi.json\ndocs: https://docs.siro.ai/getting-started\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Organization API token\n  description: 'Organization integration token from Siro admin (Person icon → API Tokens). Send\n    Authorization: Bearer <organization-api-token>. This is not the OAuth access token used\n    with api.siro.ai user-scoped endpoints.'\n  sources:\n  - openapi/siro-external-api-openapi.json\n  - openapi/siro-openapi-original.json\n- name: SiroAuthToken\n  type: apiKey\n  in: header\n  parameter: x-siro-auth-token\n  description: 'OAuth access token for user-scoped requests (Authorization Code or machine-to-machine).\n    Send header `x-siro-auth-token: <oauth-access-token>`.\
  \ Not an organization API key.'\n  sources:\n  - openapi/siro-folders-api-openapi.json\n  - openapi/siro-recordings-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/authentication/siro-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sales
- Sales Coaching
- Conversation Intelligence
- Field Sales
- CRM
- AI
- Speech to Text
- Webhooks
- Integrations
---
