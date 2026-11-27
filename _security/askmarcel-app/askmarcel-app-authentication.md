---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Ask Marcel API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ask Marcel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ask Marcel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ask Marcel
provider_slug: askmarcel-app
scheme_count: 2
schemes:
- evidence: 'Pass it as Authorization: Bearer on https://api.askmarcel.app/v1/* and https://mcp.askmarcel.app. Header Authorization: Bearer ak_live_...'
  header: Authorization
  how_to_obtain: 'Create a secret key in the authenticated developer area: https://app.askmarcel.app/developers.'
  location: header
  name: Secret API key (server/MCP)
  type: http-bearer
- authorize_url: app.askmarcel.app/api/oauth/authorize
  evidence: Authorization Code flow with dynamic client registration.
  how_to_obtain: 'Register a client dynamically via the Register endpoint: app.askmarcel.app/api/oauth/register.'
  name: OAuth 2.0 (Claude Desktop / connectors)
  token_url: app.askmarcel.app/api/oauth/token
  type: oauth2
slug: askmarcel-app-authentication
source_filename: askmarcel-app-authentication.yml
source_heading: Authentication Profile
source_url: https://askmarcel.app/fr/api/docs/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://askmarcel.app/fr/api/docs/authentication\nsources:\n- https://askmarcel.app/fr/api/docs/authentication\n- https://askmarcel.app/en/api/docs/authentication\n- https://askmarcel.app/fr/api/docs/quickstart\n- https://askmarcel.app/en/api/docs/quickstart\ndescription: Authentication methods for Ask Marcel API\nschemes:\n- type: http-bearer\n  name: Secret API key (server/MCP)\n  evidence: 'Pass it as Authorization: Bearer on https://api.askmarcel.app/v1/* and https://mcp.askmarcel.app. Header Authorization: Bearer ak_live_...'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a secret key in the authenticated developer area: https://app.askmarcel.app/developers.'\n- type: oauth2\n  name: OAuth 2.0 (Claude Desktop / connectors)\n  evidence: Authorization Code flow with dynamic client registration.\n  token_url: app.askmarcel.app/api/oauth/token\n  authorize_url:\
  \ app.askmarcel.app/api/oauth/authorize\n  how_to_obtain: 'Register a client dynamically via the Register endpoint: app.askmarcel.app/api/oauth/register.'\ndocs: https://askmarcel.app/fr/api/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/askmarcel-app/authentication/askmarcel-app-authentication.yml
summary_line: 2 schemes
tags:
- HVAC
- Engineering
- Troubleshooting
- Database
---
