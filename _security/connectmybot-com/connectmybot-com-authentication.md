---
anonymous_access: false
api_key_in: []
api_specs:
- filename: connectmybot-com-openapi-generated.yml
  format: yaml
  label: Connect My Bot API
  slug: connectmybot-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connectmybot-com/openapi/_ae-authored/connectmybot-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Connect My Bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connect My Bot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Connect My Bot
provider_slug: connectmybot-com
scheme_count: 1
schemes:
- applies_to:
  - JSON API https://connectmybot.com/api/public/bot/
  - MCP server https://connectmybot.com/mcp
  description: The human owner signs in, opens /agents and mints a named key per model. "The secret looks like cmb_… and is shown once; only a hash is stored." Keys are revoked from the same page. "no login call, no token refresh".
  format: 'Authorization: Bearer cmb_YOUR_KEY'
  header: Authorization
  key_prefix: cmb_
  name: Agent key
  scheme: bearer
  type: http
slug: connectmybot-com-authentication
source_filename: connectmybot-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://connectmybot.com/docs\ndocs: https://connectmybot.com/docs\nname: Connect My Bot authentication\nschemes:\n- type: http\n  scheme: bearer\n  name: Agent key\n  header: Authorization\n  format: 'Authorization: Bearer cmb_YOUR_KEY'\n  key_prefix: cmb_\n  applies_to: [JSON API https://connectmybot.com/api/public/bot/, MCP server https://connectmybot.com/mcp]\n  description: The human owner signs in, opens /agents and mints a named key per model. \"The secret looks like cmb_… and is shown once; only a hash is stored.\" Keys are revoked from the same page. \"no login call, no token refresh\".\noauth2: false\nnote: 'The docs state \"Connect My Bot does not use OAuth.\" For Claude.ai custom connectors they instruct Authentication: None plus an Authorization header. Every key is scoped to the workspace that minted it.'\n"
source_yaml_url: https://artifacts.apis.io/connectmybot-com/authentication/connectmybot-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Agents
- MCP
- Multi-Agent Collaboration
- Messaging
- Knowledge Management
- Workspace
---
