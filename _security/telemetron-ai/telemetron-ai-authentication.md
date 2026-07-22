---
api_key_in:
- header
api_specs:
- filename: telemetron-ai-ext-v1-openapi.yml
  format: yaml
  label: Telemetron External API (ext-v1)
  slug: telemetron-external-api-ext-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telemetron-ai/refs/heads/main/openapi/telemetron-ai-ext-v1-openapi.yml
auth_types:
- apiKey
description: 'Telemetron authenticates every External API request with a single per-organization API key. For the REST API the key is sent in the x-api-key header; the same key authenticates the hosted MCP server, where it is sent as an Authorization: Bearer token. There is no OAuth, OIDC, or per-scope model — the key grants the organization''s full API surface. Keys are issued and rotated from the dashboard (Settings > Integrations); regenerating invalidates the prior key immediately.'
kind: authentication
layout: security
method: searched
name: Telemetron Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telemetron secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Telemetron
provider_slug: telemetron-ai
scheme_count: 2
schemes:
- docs: https://docs.telemetron.ai/api-reference/introduction
  in: header
  key_name: x-api-key
  name: apiKeyAuth
  scope: organization-wide
  sources:
  - openapi/telemetron-ai-ext-v1-openapi.yml
  type: apiKey
- detail: 'Same organization API key, presented as "Authorization: Bearer <API_KEY>" to the MCP server at https://admin.telemetron.ai/api/mcp.'
  name: mcpBearer
  scheme: bearer
  sources:
  - https://docs.telemetron.ai/integrations/developer/mcp
  type: http
slug: telemetron-ai-authentication
source_filename: telemetron-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/telemetron-ai-ext-v1-openapi.yml\ndocs: https://docs.telemetron.ai/integrations/developer/api-keys\ndescription: >-\n  Telemetron authenticates every External API request with a single\n  per-organization API key. For the REST API the key is sent in the x-api-key\n  header; the same key authenticates the hosted MCP server, where it is sent as\n  an Authorization: Bearer token. There is no OAuth, OIDC, or per-scope model —\n  the key grants the organization's full API surface. Keys are issued and\n  rotated from the dashboard (Settings > Integrations); regenerating invalidates\n  the prior key immediately.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    key_name: x-api-key\n    scope: organization-wide\n    sources: [openapi/telemetron-ai-ext-v1-openapi.yml]\n    docs: https://docs.telemetron.ai/api-reference/introduction\n\
  \  - name: mcpBearer\n    type: http\n    scheme: bearer\n    detail: >-\n      Same organization API key, presented as \"Authorization: Bearer <API_KEY>\"\n      to the MCP server at https://admin.telemetron.ai/api/mcp.\n    sources: [https://docs.telemetron.ai/integrations/developer/mcp]\nkey_management:\n  issuance: Dashboard > Settings > Integrations > Developer section\n  rotation: Regenerate Key (immediately invalidates the previous key)\n  guidance: Never expose in client-side code or version control; store in env vars or a secrets manager.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telemetron-ai/refs/heads/main/authentication/telemetron-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Customer Support
- Internet of Things
- Hardware
- Telemetry
- Support Tickets
- MCP
---
