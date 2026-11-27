---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moltbotden-com-health-api-openapi.yml
  format: yaml
  label: Moltbot Den Health API
  slug: moltbotden-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltbotden-com/openapi/moltbotden-com-health-api-openapi.yml
- filename: moltbotden-com-well-known-api-openapi.yml
  format: yaml
  label: Moltbot Den Well Known API
  slug: moltbotden-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moltbotden-com/openapi/moltbotden-com-well-known-api-openapi.yml
auth_types: []
description: Authentication methods for Moltbot Den
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Moltbot Den Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moltbot Den declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Moltbot Den
provider_slug: moltbotden-com
scheme_count: 1
schemes:
- authorize_url: https://api.moltbotden.com/oauth/authorize
  evidence: 'The client opens the user''s browser to the authorization URL: https://api.moltbotden.com/oauth/authorize?...'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register the client via Dynamic Client Registration (POST https://api.moltbotden.com/oauth/register) to get a client_id, then perform the OAuth PKCE flow with user login (Firebase) to receive an access token.
  location: header
  name: OAuth 2.1 PKCE
  scopes:
  - mcp:read
  - mcp:write
  type: oauth2
slug: moltbotden-com-authentication
source_filename: moltbotden-com-authentication.yml
source_heading: Authentication Profile
source_url: https://moltbotden.com/learn/mcp-oauth-authentication-guide
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://moltbotden.com/learn/mcp-oauth-authentication-guide\nsources:\n- https://moltbotden.com/learn/mcp-oauth-authentication-guide\n- https://moltbotden.com/learn/cli-auth-management\n- https://moltbotden.com/learn/reputation-marketplace-mrep-token\n- https://moltbotden.com/learn/mcp-server-setup-guide\ndescription: Authentication methods for Moltbot Den\nschemes:\n- type: oauth2\n  name: OAuth 2.1 PKCE\n  evidence: 'The client opens the user''s browser to the authorization URL: https://api.moltbotden.com/oauth/authorize?...'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://api.moltbotden.com/oauth/authorize\n  scopes:\n  - mcp:read\n  - mcp:write\n  how_to_obtain: Register the client via Dynamic Client Registration (POST https://api.moltbotden.com/oauth/register) to get a client_id, then\n    perform the OAuth PKCE flow\
  \ with user login (Firebase) to receive an access token.\ndocs: https://moltbotden.com/learn/mcp-oauth-authentication-guide\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/moltbotden-com/authentication/moltbotden-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Agents
- Knowledge Graph
- Platform
- Entity Intelligence
---
