---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cralo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cralo declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Cralo
provider_slug: cralo-ai
scheme_count: 4
schemes:
- description: Cralo uses device authorization when you set up an agent interactively (`cralo auth login`); the CLI opens a browser, polls, and stores the credential in the OS keychain or a protected credential file.
  flow: device
  name: device-authorization
  type: oauth2
- description: Scoped API keys for unattended agents, supplied via CRALO_API_KEY; the environment value takes precedence over a stored credential. The CLI never accepts an API-key flag. Keys are created in the dashboard (https://app.cralo.ai).
  format: ot_live_<id>_<secret>
  in: environment (CRALO_API_KEY)
  name: api-key
  type: apiKey
- description: 'Remote MCP (https://mcp.cralo.ai/mcp) default flow is OAuth: the host opens Cralo, you sign in and approve the connector.'
  name: mcp-oauth
  type: oauth2
- description: Headless MCP hosts can send a Cralo API key as a bearer token instead of OAuth.
  name: mcp-bearer
  scheme: bearer
  type: http
slug: cralo-ai-authentication
source_filename: cralo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cralo.ai/docs/cli/authentication\ndocs: https://cralo.ai/docs/cli/authentication\nschemes:\n- name: device-authorization\n  type: oauth2\n  flow: device\n  description: Cralo uses device authorization when you set up an agent interactively (`cralo auth login`); the CLI opens a browser, polls, and stores the credential in the OS keychain or a protected credential\n    file.\n- name: api-key\n  type: apiKey\n  in: environment (CRALO_API_KEY)\n  format: ot_live_<id>_<secret>\n  description: Scoped API keys for unattended agents, supplied via CRALO_API_KEY; the environment value takes precedence over a stored credential. The CLI never accepts an API-key flag. Keys are created\n    in the dashboard (https://app.cralo.ai).\n- name: mcp-oauth\n  type: oauth2\n  description: 'Remote MCP (https://mcp.cralo.ai/mcp) default flow is OAuth: the host opens Cralo, you sign in and approve the connector.'\n- name: mcp-bearer\n  type:\
  \ http\n  scheme: bearer\n  description: Headless MCP hosts can send a Cralo API key as a bearer token instead of OAuth.\nnote: No OpenAPI is published, so nothing was derived from securitySchemes; the API-level wire format of the key (header name) is not documented beyond the MCP bearer statement. Auth endpoints were not\n  called.\ndocs_mcp: https://cralo.ai/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/cralo-ai/authentication/cralo-ai-authentication.yml
summary_line: 4 schemes
tags:
- Company
- AI Agents
- Agent Tools
- Pay-per-use
- CLI
- Web Scraping
- Search
- Data Enrichment
---
