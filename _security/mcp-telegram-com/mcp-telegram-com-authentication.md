---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcp-telegram-com-openapi-generated.yml
  format: yaml
  label: mcp-telegram-com API
  slug: mcp-telegram-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-telegram-com/openapi/_ae-authored/mcp-telegram-com-openapi-generated.yml
auth_types: []
description: OAuth 2.0 Authorization Code Grant with PKCE
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mcp-telegram-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: mcp-telegram-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mcp-telegram-com
provider_slug: mcp-telegram-com
scheme_count: 1
schemes:
- authorize_url: /oauth/authorize
  evidence: 'Use the access_token as Authorization: Bearer ... on /mcp requests.'
  flows:
  - authorization_code
  how_to_obtain: Register client via POST /oauth/register to receive client_id (and optional client_secret), then perform the Authorization Code with PKCE flow.
  name: OAuth 2.0
  type: oauth2
slug: mcp-telegram-com-authentication
source_filename: mcp-telegram-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp-telegram.com/docs/oauth
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp-telegram.com/docs/oauth\nsources:\n- https://mcp-telegram.com/docs/oauth\n- https://mcp-telegram.com/ru/docs/oauth\n- https://mcp-telegram.com/es/docs/oauth\n- https://mcp-telegram.com/de/docs/oauth\ndescription: OAuth 2.0 Authorization Code Grant with PKCE\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Use the access_token as Authorization: Bearer ... on /mcp requests.'\n  flows:\n  - authorization_code\n  authorize_url: /oauth/authorize\n  how_to_obtain: Register client via POST /oauth/register to receive client_id (and optional client_secret), then perform the Authorization Code\n    with PKCE flow.\ndocs: https://mcp-telegram.com/docs/oauth\n"
source_yaml_url: https://artifacts.apis.io/mcp-telegram-com/authentication/mcp-telegram-com-authentication.yml
summary_line: 1 scheme
tags:
- Telegram
- MCP
- Open Source
- Chat Analytics
---
