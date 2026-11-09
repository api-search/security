---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Demo St Authentication
name_suffix: Authentication
oauth_flows: []
overview: demo.st secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: demo.st
provider_slug: demo-st
scheme_count: 2
schemes:
- applies_to: demo.st MCP Server (https://demo.st/mcp)
  description: 'Per-user MCP token. Documented (mcp.json): "User must sign in on this site, then open https://demo.st/api/mcp/token in the browser (or GET that URL while signed in) to obtain a token." Sent as Authorization: Bearer <token>. Required for reserve_subdomain, upload_site, clear_site, release_subdomain, and document DB tools; check_subdomain_availability is documented as "No auth."'
  name: mcpBearerToken
  scheme: bearer
  sources:
  - https://demo.st/mcp.json
  token_url: https://demo.st/api/mcp/token
  type: http
- applies_to: demo.st Document API (https://api.demo.st/v1)
  description: 'Per-site public API key with prefix dk_, obtained via the get_site_api_key MCP tool or the dashboard, rotatable (rotate_site_api_key). Homepage: "Embed in your static site for https://api.demo.st/v1 as Authorization: Bearer dk_... . Requires a reserved subdomain."'
  key_prefix: dk_
  name: siteApiKeyBearer
  scheme: bearer
  sources:
  - https://demo.st/
  - https://api.demo.st/
  type: http
slug: demo-st-authentication
source_filename: demo-st-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://demo.st/mcp.json\ndocs: https://demo.st/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: mcpBearerToken\n  type: http\n  scheme: bearer\n  applies_to: demo.st MCP Server (https://demo.st/mcp)\n  description: 'Per-user MCP token. Documented (mcp.json): \"User must sign in on this site, then open https://demo.st/api/mcp/token in the browser (or GET that URL while signed in) to obtain a token.\" Sent\n    as Authorization: Bearer <token>. Required for reserve_subdomain, upload_site, clear_site, release_subdomain, and document DB tools; check_subdomain_availability is documented as \"No auth.\"'\n  token_url: https://demo.st/api/mcp/token\n  sources:\n  - https://demo.st/mcp.json\n- name: siteApiKeyBearer\n  type: http\n  scheme: bearer\n  applies_to: demo.st Document API (https://api.demo.st/v1)\n  description: 'Per-site public API key with prefix dk_, obtained via the get_site_api_key MCP tool or the dashboard, rotatable\
  \ (rotate_site_api_key). Homepage: \"Embed in your static site for https://api.demo.st/v1\n    as Authorization: Bearer dk_... . Requires a reserved subdomain.\"'\n  key_prefix: dk_\n  sources:\n  - https://demo.st/\n  - https://api.demo.st/\nnote: 'Sign-in to the website itself is via Google, GitHub OAuth or email/password; those flows were not called. No OpenAPI securitySchemes exist (no contract is published). api.demo.st also exposes /admin/*\n  guarded by X-Demo-Service-Secret, which is operator-internal and not a customer auth scheme. apis.yml describes an X-Demo-Key header alternative for the document API, but the API root fetched 2026-11-05\n  names only \"Authorization: Bearer dk_...\", so that header is not recorded as a scheme here.'\n"
source_yaml_url: https://artifacts.apis.io/demo-st/authentication/demo-st-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Hosting
- Static Site Hosting
- Prototyping
- MCP
- AI Agents
- Developer Tools
- Document-Api
---
