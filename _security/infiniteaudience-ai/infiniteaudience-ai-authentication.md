---
anonymous_access: false
api_key_in: []
api_specs:
- filename: infiniteaudience-ai-a2a-api-openapi.yml
  format: yaml
  label: Infinite Audience A2A API
  slug: infiniteaudience-ai-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-a2a-api-openapi.yml
- filename: infiniteaudience-ai-account-api-openapi.yml
  format: yaml
  label: Infinite Audience Account API
  slug: infiniteaudience-ai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-account-api-openapi.yml
- filename: infiniteaudience-ai-audiences-api-openapi.yml
  format: yaml
  label: Infinite Audience Audiences API
  slug: infiniteaudience-ai-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-audiences-api-openapi.yml
- filename: infiniteaudience-ai-auth-api-openapi.yml
  format: yaml
  label: Infinite Audience Auth API
  slug: infiniteaudience-ai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-auth-api-openapi.yml
- filename: infiniteaudience-ai-campaigns-api-openapi.yml
  format: yaml
  label: Infinite Audience Campaigns API
  slug: infiniteaudience-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-campaigns-api-openapi.yml
- filename: infiniteaudience-ai-deliveries-api-openapi.yml
  format: yaml
  label: Infinite Audience Deliveries API
  slug: infiniteaudience-ai-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-deliveries-api-openapi.yml
- filename: infiniteaudience-ai-discovery-api-openapi.yml
  format: yaml
  label: Infinite Audience Discovery API
  slug: infiniteaudience-ai-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-discovery-api-openapi.yml
- filename: infiniteaudience-ai-enrichment-api-openapi.yml
  format: yaml
  label: Infinite Audience Enrichment API
  slug: infiniteaudience-ai-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-enrichment-api-openapi.yml
- filename: infiniteaudience-ai-integrations-api-openapi.yml
  format: yaml
  label: Infinite Audience Integrations API
  slug: infiniteaudience-ai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-integrations-api-openapi.yml
- filename: infiniteaudience-ai-mcp-api-openapi.yml
  format: yaml
  label: Infinite Audience MCP API
  slug: infiniteaudience-ai-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-mcp-api-openapi.yml
- filename: infiniteaudience-ai-oauth-api-openapi.yml
  format: yaml
  label: Infinite Audience OAuth API
  slug: infiniteaudience-ai-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-oauth-api-openapi.yml
- filename: infiniteaudience-ai-partnerships-api-openapi.yml
  format: yaml
  label: Infinite Audience Partnerships API
  slug: infiniteaudience-ai-partnerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-partnerships-api-openapi.yml
- filename: infiniteaudience-ai-segments-api-openapi.yml
  format: yaml
  label: Infinite Audience Segments API
  slug: infiniteaudience-ai-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-segments-api-openapi.yml
- filename: infiniteaudience-ai-settings-api-openapi.yml
  format: yaml
  label: Infinite Audience Settings API
  slug: infiniteaudience-ai-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-settings-api-openapi.yml
- filename: infiniteaudience-ai-triggers-api-openapi.yml
  format: yaml
  label: Infinite Audience Triggers API
  slug: infiniteaudience-ai-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-triggers-api-openapi.yml
- filename: infiniteaudience-ai-webhooks-api-openapi.yml
  format: yaml
  label: Infinite Audience Webhooks API
  slug: infiniteaudience-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-webhooks-api-openapi.yml
- filename: infiniteaudience-ai-workflows-api-openapi.yml
  format: yaml
  label: Infinite Audience Workflows API
  slug: infiniteaudience-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/openapi/infiniteaudience-ai-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Infiniteaudience Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infinite Audience secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infinite Audience
provider_slug: infiniteaudience-ai
scheme_count: 1
schemes:
- bearerFormat: OAuth access token
  description: Person-bound MCP OAuth bearer with the openid scope for UserInfo.
  name: oidcBearer
  scheme: bearer
  sources:
  - openapi/infiniteaudience-ai-openapi.yml
  type: http
slug: infiniteaudience-ai-authentication
source_filename: infiniteaudience-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/infiniteaudience-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oidcBearer\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth access token\n  description: Person-bound MCP OAuth bearer with the openid scope for UserInfo.\n  sources:\n  - openapi/infiniteaudience-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infiniteaudience-ai/refs/heads/main/authentication/infiniteaudience-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Identity Resolution
- Data Enrichment
- Audiences
- Marketing
- MCP
- A2A
---
