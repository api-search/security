---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deoochform Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deoochform declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Deoochform
provider_slug: deoochform-com
scheme_count: 2
schemes:
- authorization_url: https://deoochform.com/authorize
  confidential_clients: registered by arrangement; client_secret presented at /token as HTTP Basic or body parameters
  dynamic_client_registration: RFC 7591, optional, public clients
  flows:
  - authorizationCode
  header: 'Authorization: Bearer <token>'
  id: oauth2
  metadata_url: https://deoochform.com/.well-known/oauth-authorization-server
  pkce: S256 (required for public clients)
  quote: Everything is JSON over HTTPS, and every request carries an OAuth bearer token. There are no API keys to paste anywhere.
  registration_url: https://deoochform.com/register
  token_lifetime: Tokens do not expire; revoked from Settings, API tokens. No refresh grant.
  token_prefix: dff_
  token_type: bearer
  token_url: https://deoochform.com/token
  type: oauth2
- applies_to: https://deoochform.com/api/mcp
  description: The remote MCP server authenticates with OAuth (no API key); the first tool call opens a browser for sign in.
  id: mcp-oauth
  source: https://deoochform.com/help/mcp-server
  type: oauth2
slug: deoochform-com-authentication
source_filename: deoochform-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Deoochform authentication\ngenerated: '2026-11-05'\nmethod: searched\nsource: https://deoochform.com/help/api\ndocs: https://deoochform.com/help/api\nschemes:\n- id: oauth2\n  type: oauth2\n  flows:\n  - authorizationCode\n  authorization_url: https://deoochform.com/authorize\n  token_url: https://deoochform.com/token\n  registration_url: https://deoochform.com/register\n  metadata_url: https://deoochform.com/.well-known/oauth-authorization-server\n  pkce: S256 (required for public clients)\n  dynamic_client_registration: RFC 7591, optional, public clients\n  confidential_clients: registered by arrangement; client_secret presented at /token as HTTP Basic or body parameters\n  token_type: bearer\n  token_prefix: dff_\n  token_lifetime: Tokens do not expire; revoked from Settings, API tokens. No refresh grant.\n  header: 'Authorization: Bearer <token>'\n  quote: Everything is JSON over HTTPS, and every request carries an OAuth bearer token. There are no API keys to paste\
  \ anywhere.\n- id: mcp-oauth\n  type: oauth2\n  applies_to: https://deoochform.com/api/mcp\n  description: The remote MCP server authenticates with OAuth (no API key); the first tool call opens a browser for sign in.\n  source: https://deoochform.com/help/mcp-server\napi_keys: none\nnote: Auth endpoints were read from the docs only; none were called.\n"
source_yaml_url: https://artifacts.apis.io/deoochform-com/authentication/deoochform-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Forms
- Form Builder
- Surveys
- Artificial Intelligence
- MCP
- Payments
- Webhook
- No-Code
---
