---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cleotic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleotic declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cleotic
provider_slug: cleotic-ai
scheme_count: 3
schemes:
- description: OAuth sign-in in the browser; choose the organisation at sign-in. No client ID or secret is needed. "Cleotic API keys and X-API-Key aren't accepted." Unauthenticated calls return auth_required.
  docs: https://cleotic.ai/docs/integrations/connected-agents
  name: mcp-oauth
  surface: Connected Agents MCP (https://mcp.cleotic.ai)
  type: oauth2
- description: cleotic auth login opens the browser (or device link + code over SSH); session kept in the system keychain and refreshed automatically.
  docs: https://cleotic.ai/docs/integrations/cli
  name: cli-browser-session
  surface: Cleotic CLI
  type: oauth2
- description: Create a key in Settings → CLI API keys and set CLEOTIC_API_KEY for CI and scripts. The header or transport for the key is not documented.
  docs: https://cleotic.ai/docs/integrations/cli
  name: cli-api-key
  surface: Cleotic CLI / Cleotic API (https://api.cleotic.ai)
  type: apiKey
slug: cleotic-ai-authentication
source_filename: cleotic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://cleotic.ai/docs/integrations/connected-agents\n- https://cleotic.ai/docs/integrations/cli\ndocs: https://cleotic.ai/docs/integrations/connected-agents\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  surface: Connected Agents MCP (https://mcp.cleotic.ai)\n  description: OAuth sign-in in the browser; choose the organisation at sign-in. No client ID or secret is needed. \"Cleotic API keys and X-API-Key aren't accepted.\" Unauthenticated calls return auth_required.\n  docs: https://cleotic.ai/docs/integrations/connected-agents\n- name: cli-browser-session\n  type: oauth2\n  surface: Cleotic CLI\n  description: cleotic auth login opens the browser (or device link + code over SSH); session kept in the system keychain and refreshed automatically.\n  docs: https://cleotic.ai/docs/integrations/cli\n- name: cli-api-key\n  type: apiKey\n  surface: Cleotic CLI / Cleotic API (https://api.cleotic.ai)\n  description: Create a key\
  \ in Settings → CLI API keys and set CLEOTIC_API_KEY for CI and scripts. The header or transport for the key is not documented.\n  docs: https://cleotic.ai/docs/integrations/cli\nnote: No public REST API reference or OpenAPI is published; the API host is named only as the CLI default api_url. OAuth scopes are not documented; access follows the organisation role and brand access.\n"
source_yaml_url: https://artifacts.apis.io/cleotic-ai/authentication/cleotic-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Visibility
- Answer Engine Optimization
- Generative Engine Optimization
- SEO
- Brand Monitoring
- Content Management
- MCP
- CLI
---
