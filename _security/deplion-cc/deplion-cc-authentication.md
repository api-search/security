---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deplion Cc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deplion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Deplion
provider_slug: deplion-cc
scheme_count: 2
schemes:
- applies_to: https://deplion.cc/mcp/deplion
  authorization_servers:
  - https://deplion.cc
  description: The first time it reaches Deplion, it opens a browser window and asks you to authorize the connection. Approve it while signed in to your Deplion account, and the client stores the authorization itself.
  evidence: 'GET https://deplion.cc/.well-known/oauth-protected-resource -> 200 {resource: https://deplion.cc, authorization_servers: [https://deplion.cc], scopes_supported: [mcp:use]} (2026-11-05)'
  name: oauth2-browser-authorization
  scopes:
  - mcp:use
  type: oauth2
- applies_to: https://deplion.cc/mcp/deplion
  description: Some clients don't support the browser authorization flow yet. For those, Deplion still issues a personal access token.
  issuance: Settings -> MCP access -> Create token; shown once, stored only as a hash.
  name: personal-access-token
  note: The docs say to keep the token in the client's secret storage. They do not name the header; bearer is our reading of how MCP clients send tokens and has not been checked against a live call.
  privilege: It grants full access to your projects and your form submissions.
  revocation: revocation takes effect immediately
  rotation: To replace a token, use Rotate token. The old and new tokens both stay active, so nothing breaks while you update your clients.
  scheme: bearer
  type: http
slug: deplion-cc-authentication
source_filename: deplion-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://docs.deplion.cc/s/documentations/doc/connect-your-ai-assistant-7Pwj7bazqW\ndocs: https://docs.deplion.cc/s/documentations/doc/connect-your-ai-assistant-7Pwj7bazqW\nprotected_resource_metadata: https://deplion.cc/.well-known/oauth-protected-resource\nschemes:\n- name: oauth2-browser-authorization\n  type: oauth2\n  applies_to: https://deplion.cc/mcp/deplion\n  authorization_servers:\n  - https://deplion.cc\n  scopes:\n  - mcp:use\n  description: \"The first time it reaches Deplion, it opens a browser window and asks you to authorize the connection. Approve it while signed in to your Deplion account, and the client stores the authorization itself.\"\n  evidence: \"GET https://deplion.cc/.well-known/oauth-protected-resource -> 200 {resource: https://deplion.cc, authorization_servers: [https://deplion.cc], scopes_supported: [mcp:use]} (2026-11-05)\"\n- name: personal-access-token\n  type: http\n  scheme: bearer\n  applies_to:\
  \ https://deplion.cc/mcp/deplion\n  description: \"Some clients don't support the browser authorization flow yet. For those, Deplion still issues a personal access token.\"\n  issuance: Settings -> MCP access -> Create token; shown once, stored only as a hash.\n  rotation: \"To replace a token, use Rotate token. The old and new tokens both stay active, so nothing breaks while you update your clients.\"\n  revocation: revocation takes effect immediately\n  privilege: \"It grants full access to your projects and your form submissions.\"\n  note: The docs say to keep the token in the client's secret storage. They do not name the header; bearer is our reading of how MCP clients send tokens and has not been checked against a live call.\ntransport: streamable HTTP only (\"stdio and SSE are not supported\")\n"
source_yaml_url: https://artifacts.apis.io/deplion-cc/authentication/deplion-cc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- MCP
- Website Publishing
- Web Hosting
- Deployment
- No-Code
- AI Agents
---
