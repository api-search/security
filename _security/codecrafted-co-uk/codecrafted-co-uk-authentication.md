---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CodeCrafted Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeCrafted declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CodeCrafted
provider_slug: codecrafted-co-uk
scheme_count: 2
schemes:
- authorization_servers:
  - https://design.codecrafted.co.uk
  description: Interactive MCP clients use OAuth; "OAuth-capable clients discover the sign-in flow." Connections are revocable from the dashboard.
  discovery: https://design.codecrafted.co.uk/.well-known/oauth-protected-resource
  discovery_http_status: 200
  name: oauth2
  scopes:
  - mcp:use
  type: oauth2
- description: API keys remain available for CI and unattended automation; "For clients without OAuth, use their secret mechanism to supply an API key as a Bearer token." Personal API keys are shown once and stored as one-way hashes, and can be revoked.
  docs: https://design.codecrafted.co.uk/security
  name: apiKey
  scheme: bearer
  type: http
slug: codecrafted-co-uk-authentication
source_filename: codecrafted-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://design.codecrafted.co.uk/docs\ndocs: https://design.codecrafted.co.uk/docs\nnote: No OpenAPI is published; profile read from the docs, the security page and the live OAuth protected-resource metadata (RFC 9728) at /.well-known/oauth-protected-resource (HTTP 200).\nschemes:\n- name: oauth2\n  type: oauth2\n  description: 'Interactive MCP clients use OAuth; \"OAuth-capable clients discover the sign-in flow.\" Connections are revocable from the dashboard.'\n  authorization_servers:\n  - https://design.codecrafted.co.uk\n  scopes:\n  - mcp:use\n  discovery: https://design.codecrafted.co.uk/.well-known/oauth-protected-resource\n  discovery_http_status: 200\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'API keys remain available for CI and unattended automation; \"For clients without OAuth, use their secret mechanism to supply an API key as a Bearer token.\" Personal API keys are shown once and stored as\
  \ one-way hashes, and can be revoked.'\n  docs: https://design.codecrafted.co.uk/security\n"
source_yaml_url: https://artifacts.apis.io/codecrafted-co-uk/authentication/codecrafted-co-uk-authentication.yml
summary_line: 2 schemes
tags:
- Company
- MCP
- AI Agents
- Design Systems
- Web Development
- Software Development
- Hosting
- United Kingdom
---
