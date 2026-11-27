---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coderbuds-com-openapi-generated.yml
  format: yaml
  label: Coderbuds API
  slug: coderbuds-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderbuds-com/openapi/_ae-authored/coderbuds-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Coderbuds Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coderbuds declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Coderbuds
provider_slug: coderbuds-com
scheme_count: 4
schemes:
- applies_to: REST API (https://coderbuds.com/api/v1)
  description: Every request carries Authorization Bearer <token>; send Accept application/json too so validation failures come back as JSON rather than a redirect. Tokens are minted on the API Tokens page (https://coderbuds.com/user/api-tokens), belong to a person, see what that person's team memberships allow, do not expire on a timer and can be revoked at any time (next request gets 401). The read permission is required and sufficient; permissions cannot be added to an existing token.
  header: 'Authorization: Bearer <token>'
  name: bearer
  scheme: bearer
  token_management: https://coderbuds.com/user/api-tokens
  type: http
- applies_to: MCP server (https://coderbuds.com/mcp/insights)
  description: Default MCP auth is OAuth in the browser ("I sign in to Coderbuds in the browser and click Authorize, once per person, per machine"). No token to mint or store.
  docs: https://coderbuds.com/docs/mcp
  name: mcp-oauth
  type: oauth2
- applies_to: MCP server, headless environments (CI, servers)
  description: Fallback only where a browser cannot open; pass --header "Authorization Bearer <your-token>". A token is tied to the user personally.
  docs: https://coderbuds.com/docs/mcp
  name: mcp-bearer-fallback
  scheme: bearer
  type: http
- applies_to: Inbound deploy webhook POST /api/deploy-events/{repository}/{token}
  description: A per-repository token embedded in the webhook URL is the only credential the endpoint accepts; a wrong or missing token returns 404. Rotatable with --rotate on the Artisan command.
  docs: https://coderbuds.com/docs/deploy-hooks
  in: path
  name: deploy-webhook-url-token
  type: apiKey
slug: coderbuds-com-authentication
source_filename: coderbuds-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coderbuds.com/docs/api\ndocs: https://coderbuds.com/docs/api\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  applies_to: REST API (https://coderbuds.com/api/v1)\n  header: 'Authorization: Bearer <token>'\n  description: Every request carries Authorization Bearer <token>; send Accept application/json too so validation failures come back as JSON rather than a redirect. Tokens are minted on the API Tokens page (https://coderbuds.com/user/api-tokens), belong to a person, see what that person's team memberships allow, do not expire on a timer and can be revoked at any time (next request gets 401). The read permission is required and sufficient; permissions cannot be added to an existing token.\n  token_management: https://coderbuds.com/user/api-tokens\n- name: mcp-oauth\n  type: oauth2\n  applies_to: MCP server (https://coderbuds.com/mcp/insights)\n  docs: https://coderbuds.com/docs/mcp\n  description: Default\
  \ MCP auth is OAuth in the browser (\"I sign in to Coderbuds in the browser and click Authorize, once per person, per machine\"). No token to mint or store.\n- name: mcp-bearer-fallback\n  type: http\n  scheme: bearer\n  applies_to: MCP server, headless environments (CI, servers)\n  docs: https://coderbuds.com/docs/mcp\n  description: Fallback only where a browser cannot open; pass --header \"Authorization Bearer <your-token>\". A token is tied to the user personally.\n- name: deploy-webhook-url-token\n  type: apiKey\n  in: path\n  applies_to: Inbound deploy webhook POST /api/deploy-events/{repository}/{token}\n  docs: https://coderbuds.com/docs/deploy-hooks\n  description: A per-repository token embedded in the webhook URL is the only credential the endpoint accepts; a wrong or missing token returns 404. Rotatable with --rotate on the Artisan command.\n"
source_yaml_url: https://artifacts.apis.io/coderbuds-com/authentication/coderbuds-com-authentication.yml
summary_line: 4 schemes
tags:
- Company
- DORA Metrics
- Engineering Metrics
- Developer Productivity
- Code Review
- AI Agents
- MCP
- Software Engineering Intelligence
---
