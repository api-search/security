---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'NoteFit uses OAuth 2.1 authorization code flow with PKCE. Access tokens are sent as an Authorization: Bearer header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NoteFit Authentication
name_suffix: Authentication
oauth_flows: []
overview: NoteFit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NoteFit
provider_slug: notefit-app
scheme_count: 1
schemes:
- authorize_url: https://notefit.app/api/mcp/oauth/authorize
  evidence: Clients authenticate with OAuth 2.1 and register themselves — there are no API keys to request and no sales contact in the way.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Dynamic client registration at https://notefit.app/api/mcp/oauth/register
  location: header
  name: Bearer
  scopes:
  - notefit:read
  - notefit:write
  type: http-bearer
slug: notefit-app-authentication
source_filename: notefit-app-authentication.yml
source_heading: Authentication Profile
source_url: https://notefit.app/developers
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://notefit.app/developers\nsources:\n- https://notefit.app/developers\n- https://notefit.app/.well-known/oauth-protected-resource\n- https://notefit.app/.well-known/oauth-authorization-server\ndescription: 'NoteFit uses OAuth 2.1 authorization code flow with PKCE. Access tokens are sent as an Authorization: Bearer header.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Clients authenticate with OAuth 2.1 and register themselves — there are no API keys to request and no sales contact in the way.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://notefit.app/api/mcp/oauth/authorize\n  scopes:\n  - notefit:read\n  - notefit:write\n  how_to_obtain: Dynamic client registration at https://notefit.app/api/mcp/oauth/register\ndocs: https://notefit.app/developers\n"
source_yaml_url: https://artifacts.apis.io/notefit-app/authentication/notefit-app-authentication.yml
summary_line: 1 scheme
tags:
- Fitness
- Coaching
- Training
- Sports
- Health
---
