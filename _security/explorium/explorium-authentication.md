---
api_key_in: []
api_specs:
- filename: explorium-business-enrichments-api-openapi.yml
  format: yaml
  label: Explorium Business Enrichments API
  slug: explorium-business-enrichments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-business-enrichments-api-openapi.yml
- filename: explorium-businesses-api-openapi.yml
  format: yaml
  label: Explorium Businesses API
  slug: explorium-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-businesses-api-openapi.yml
- filename: explorium-credits-api-openapi.yml
  format: yaml
  label: Explorium Credits API
  slug: explorium-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-credits-api-openapi.yml
- filename: explorium-events-api-openapi.yml
  format: yaml
  label: Explorium Events API
  slug: explorium-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-events-api-openapi.yml
- filename: explorium-prospect-enrichments-api-openapi.yml
  format: yaml
  label: Explorium Prospect Enrichments API
  slug: explorium-prospect-enrichments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-prospect-enrichments-api-openapi.yml
- filename: explorium-prospects-api-openapi.yml
  format: yaml
  label: Explorium Prospects API
  slug: explorium-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-prospects-api-openapi.yml
- filename: explorium-webhooks-api-openapi.yml
  format: yaml
  label: Explorium Webhooks API
  slug: explorium-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Explorium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Explorium secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Explorium
provider_slug: explorium
scheme_count: 1
schemes:
- description: API key issued in the Explorium admin portal at https://admin.explorium.ai/api-key and sent in the API_KEY request header on every call to https://api.explorium.ai. The same key authorizes the AgentSource REST API and, for Docker self-hosting, the AgentSource MCP server (passed as API_ACCESS_TOKEN). Remote MCP connections authorize through the connected client rather than a raw header.
  in: header
  keyName: API_KEY
  name: apiKeyHeader
  sources:
  - openapi/explorium-openapi.yml
  - https://developers.explorium.ai/reference/fetch_businesses
  - https://github.com/explorium-ai/mcp-explorium
  type: apiKey
slug: explorium-authentication
source_filename: explorium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/explorium-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  keyName: API_KEY\n  description: >-\n    API key issued in the Explorium admin portal at\n    https://admin.explorium.ai/api-key and sent in the API_KEY request header on\n    every call to https://api.explorium.ai. The same key authorizes the\n    AgentSource REST API and, for Docker self-hosting, the AgentSource MCP\n    server (passed as API_ACCESS_TOKEN). Remote MCP connections authorize\n    through the connected client rather than a raw header.\n  sources:\n  - openapi/explorium-openapi.yml\n  - https://developers.explorium.ai/reference/fetch_businesses\n  - https://github.com/explorium-ai/mcp-explorium\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/authentication/explorium-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Enrichment
- Web Intelligence
- Reference Data
- B2B Data
- Company Data
- AI Agents
- Prospect Enrichment
- Firmographics
- MCP
---
