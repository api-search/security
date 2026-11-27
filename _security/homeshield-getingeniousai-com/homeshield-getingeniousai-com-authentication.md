---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for HomeShield MCP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HomeShield MCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: HomeShield MCP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HomeShield MCP
provider_slug: homeshield-getingeniousai-com
scheme_count: 1
schemes:
- evidence: 'The short answer: A reverse proxy protects a home MCP server by standing between the internet and the server, on the public port, and refusing to forward any request that does not carry the right credentials.'
  header: Authorization
  location: header
  name: Basic Auth
  type: http-basic
slug: homeshield-getingeniousai-com-authentication
source_filename: homeshield-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://homeshield.getingeniousai.com/guides/how-to-put-authentication-in-front-of-mcp-server
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://homeshield.getingeniousai.com/guides/how-to-put-authentication-in-front-of-mcp-server\nsources:\n- https://homeshield.getingeniousai.com/guides/how-to-put-authentication-in-front-of-mcp-server\n- https://homeshield.getingeniousai.com/guides/oauth-protected-resource-mcp-server\n- https://homeshield.getingeniousai.com/guides/api-keys-and-tokens-on-home-mcp-servers\n- https://homeshield.getingeniousai.com/guides/reverse-proxy-basic-auth-home-server\ndescription: Authentication schemes for HomeShield MCP\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: 'The short answer: A reverse proxy protects a home MCP server by standing between the internet and the server, on the public port,\n    and refusing to forward any request that does not carry the right credentials.'\n  location: header\n  header: Authorization\ndocs: https://homeshield.getingeniousai.com/guides/how-to-put-authentication-in-front-of-mcp-server\n"
source_yaml_url: https://artifacts.apis.io/homeshield-getingeniousai-com/authentication/homeshield-getingeniousai-com-authentication.yml
summary_line: 1 scheme
tags:
- Home AI
- Security
- Privacy
- Monitoring
---
