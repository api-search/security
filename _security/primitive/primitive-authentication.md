---
api_key_in:
- query
api_specs:
- filename: primitive-account-api-openapi.yml
  format: yaml
  label: Primitive Account API
  slug: primitive-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-account-api-openapi.yml
- filename: primitive-agent-api-openapi.yml
  format: yaml
  label: Primitive Agent API
  slug: primitive-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-agent-api-openapi.yml
- filename: primitive-cli-api-openapi.yml
  format: yaml
  label: Primitive CLI API
  slug: primitive-cli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-cli-api-openapi.yml
- filename: primitive-demo-api-openapi.yml
  format: yaml
  label: Primitive Demo API
  slug: primitive-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-demo-api-openapi.yml
- filename: primitive-discovery-api-openapi.yml
  format: yaml
  label: Primitive Discovery API
  slug: primitive-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-discovery-api-openapi.yml
- filename: primitive-domains-api-openapi.yml
  format: yaml
  label: Primitive Domains API
  slug: primitive-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-domains-api-openapi.yml
- filename: primitive-emails-api-openapi.yml
  format: yaml
  label: Primitive Emails API
  slug: primitive-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-emails-api-openapi.yml
- filename: primitive-endpoints-api-openapi.yml
  format: yaml
  label: Primitive Endpoints API
  slug: primitive-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-endpoints-api-openapi.yml
- filename: primitive-filters-api-openapi.yml
  format: yaml
  label: Primitive Filters API
  slug: primitive-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-filters-api-openapi.yml
- filename: primitive-functions-api-openapi.yml
  format: yaml
  label: Primitive Functions API
  slug: primitive-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-functions-api-openapi.yml
- filename: primitive-inbox-api-openapi.yml
  format: yaml
  label: Primitive Inbox API
  slug: primitive-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-inbox-api-openapi.yml
- filename: primitive-memories-api-openapi.yml
  format: yaml
  label: Primitive Memories API
  slug: primitive-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-memories-api-openapi.yml
- filename: primitive-payments-api-openapi.yml
  format: yaml
  label: Primitive Payments API
  slug: primitive-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-payments-api-openapi.yml
- filename: primitive-registries-api-openapi.yml
  format: yaml
  label: Primitive Registries API
  slug: primitive-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-registries-api-openapi.yml
- filename: primitive-routes-api-openapi.yml
  format: yaml
  label: Primitive Routes API
  slug: primitive-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-routes-api-openapi.yml
- filename: primitive-search-api-openapi.yml
  format: yaml
  label: Primitive Search API
  slug: primitive-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-search-api-openapi.yml
- filename: primitive-sending-api-openapi.yml
  format: yaml
  label: Primitive Sending API
  slug: primitive-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-sending-api-openapi.yml
- filename: primitive-service-api-openapi.yml
  format: yaml
  label: Primitive Service API
  slug: primitive-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-service-api-openapi.yml
- filename: primitive-templates-api-openapi.yml
  format: yaml
  label: Primitive Templates API
  slug: primitive-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-templates-api-openapi.yml
- filename: primitive-threads-api-openapi.yml
  format: yaml
  label: Primitive Threads API
  slug: primitive-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-threads-api-openapi.yml
- filename: primitive-wake-api-openapi.yml
  format: yaml
  label: Primitive Wake API
  slug: primitive-wake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-wake-api-openapi.yml
- filename: primitive-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Primitive Webhook Deliveries API
  slug: primitive-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/openapi/primitive-webhook-deliveries-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Primitive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Primitive secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Primitive
provider_slug: primitive
scheme_count: 2
schemes:
- description: 'API key with `prim_` prefix or OAuth access token with `prim_oat_` prefix: `Authorization: Bearer <token>`. Access is governed by the caller''s organization role (`owner`, `admin`, or `member`): API keys always act at `member` level regardless of who created them, and OAuth access tokens act with the authorizing user''s current organization role, resolved per request. Every operation in this spec is'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/primitive-openapi-original.json
  type: http
- description: Signed download token provided in webhook payloads
  in: query
  name: DownloadToken
  parameter: token
  sources:
  - openapi/primitive-openapi-original.json
  type: apiKey
slug: primitive-authentication
source_filename: primitive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/primitive-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key with `prim_` prefix or OAuth access token with `prim_oat_` prefix: `Authorization:\n    Bearer <token>`. Access is governed by the caller''s organization role (`owner`, `admin`,\n    or `member`): API keys always act at `member` level regardless of who created them, and\n    OAuth access tokens act with the authorizing user''s current organization role, resolved\n    per request. Every operation in this spec is'\n  sources:\n  - openapi/primitive-openapi-original.json\n- name: DownloadToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Signed download token provided in webhook payloads\n  sources:\n  - openapi/primitive-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primitive/refs/heads/main/authentication/primitive-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email
- Email Infrastructure
- AI Agents
- Agent Infrastructure
- Messaging
- Webhooks
- MCP
- Developer Tools
- API
---
