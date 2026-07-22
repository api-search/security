---
api_key_in:
- env
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Waniwani Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Waniwani secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Waniwani
provider_slug: waniwani
scheme_count: 2
schemes:
- applies_to:
  - '@waniwani/cli (waniwani login browser OAuth2 PKCE)'
  - hosted MCP server (mcp.waniwani.ai, eu.mcp.waniwani.ai)
  authorization_servers:
  - https://app.waniwani.ai
  bearer_methods:
  - header
  name: OAuth2.1
  notes: CLI stores access/refresh tokens in .waniwani/settings.json and auto-refreshes on 401.
  pkce: true
  scopes_ref: scopes/waniwani-scopes.yml
  type: oauth2
  version: '2.1'
- applies_to:
  - '@waniwani/sdk hosted tier (hosted flow state, tracking, KB, chat widget)'
  - CI / long-lived programmatic access as an alternative to OAuth tokens
  env: WANIWANI_API_KEY
  key_prefix: wwk_
  name: ApiKey
  notes: Optional. OSS flow engine runs with no key; WANIWANI_API_KEY opts into the hosted Platform.
  type: apiKey
slug: waniwani-authentication
source_filename: waniwani-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.waniwani.ai/mcp-server/connect\ndocs: https://docs.waniwani.ai/sdk/configuration/environment-variables\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [authorizationCode]\n  oauth2_version: \"2.1\"\n  api_key_in: [env, header]\nschemes:\n  - name: OAuth2.1\n    type: oauth2\n    version: \"2.1\"\n    pkce: true\n    applies_to:\n      - \"@waniwani/cli (waniwani login browser OAuth2 PKCE)\"\n      - \"hosted MCP server (mcp.waniwani.ai, eu.mcp.waniwani.ai)\"\n    authorization_servers: [https://app.waniwani.ai]\n    bearer_methods: [header]\n    scopes_ref: scopes/waniwani-scopes.yml\n    notes: \"CLI stores access/refresh tokens in .waniwani/settings.json and auto-refreshes on 401.\"\n  - name: ApiKey\n    type: apiKey\n    key_prefix: \"wwk_\"\n    env: WANIWANI_API_KEY\n    applies_to:\n      - \"@waniwani/sdk hosted tier (hosted flow state, tracking, KB, chat widget)\"\n      - \"CI / long-lived programmatic\
  \ access as an alternative to OAuth tokens\"\n    notes: \"Optional. OSS flow engine runs with no key; WANIWANI_API_KEY opts into the hosted Platform.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waniwani/refs/heads/main/authentication/waniwani-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Model Context Protocol
- AI Distribution
- Conversational AI
- Lead Generation
- Insurance
- Fintech
- Agents
- SDK
---
