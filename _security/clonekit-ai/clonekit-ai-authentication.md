---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clonekit-ai-openapi-generated.yml
  format: yaml
  label: CloneKit REST API
  slug: clonekit-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clonekit-ai/openapi/_ae-authored/clonekit-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CloneKit Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloneKit declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CloneKit
provider_slug: clonekit-ai
scheme_count: 2
schemes:
- applies_to:
  - REST API https://clonekit.ai/api/v1
  - MCP https://clonekit.ai/mcp
  - clonekit-cli
  description: Make an API key in Dashboard → Connections and send it with every request. Search and public kits also work without a key.
  header: 'Authorization: Bearer ck_…'
  issued_at: https://clonekit.ai/dashboard/connections
  key_prefix: ck_
  name: bearerApiKey
  scheme: bearer
  type: http
- applies_to:
  - MCP https://clonekit.ai/mcp
  description: The first time, sign in to CloneKit and tap Allow. The docs describe a browser sign-in from the AI app; they publish no scope list, endpoints or flow name.
  name: mcpOAuthSignIn
  type: oauth2
slug: clonekit-ai-authentication
source_filename: clonekit-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clonekit.ai/docs.md\ndocs: https://clonekit.ai/docs#auth\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  applies_to: [REST API https://clonekit.ai/api/v1, MCP https://clonekit.ai/mcp, clonekit-cli]\n  key_prefix: ck_\n  header: 'Authorization: Bearer ck_…'\n  issued_at: https://clonekit.ai/dashboard/connections\n  description: Make an API key in Dashboard → Connections and send it with every request. Search and public kits also work without a key.\n- name: mcpOAuthSignIn\n  type: oauth2\n  applies_to: [MCP https://clonekit.ai/mcp]\n  description: 'The first time, sign in to CloneKit and tap Allow. The docs describe a browser sign-in from the AI app; they publish no scope list, endpoints or flow name.'\nanonymous_access:\n- REST search and public kits work without a key.\n- 'MCP tools search_kits, get_kit, get_file, check_tools and whoami are listed signed out.'\n- https://clonekit.ai/mcp/read never\
  \ signs in and serves only public kits.\n"
source_yaml_url: https://artifacts.apis.io/clonekit-ai/authentication/clonekit-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- MCP
- Marketplace
- Playbooks
- Automation
---
