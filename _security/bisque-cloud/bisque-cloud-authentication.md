---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bisque-cloud-api-openapi.json
  format: json
  label: Bisque API API
  slug: bisque-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bisque-cloud/openapi/_original/bisque-cloud-api-openapi.json
auth_types: []
description: Authentication schemes for Bisque API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bisque Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bisque declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bisque
provider_slug: bisque-cloud
scheme_count: 2
schemes:
- evidence: 'Both credentials go in the same header, on every call to the REST API and to the presentations MCP server: Authorization: Bearer <credential>'
  header: Authorization
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://bisque.cloud/oauth/authorize
  evidence: Bisque is an OAuth 2.1 authorization server with PKCE (S256) and dynamic client registration; the issuer is https://bisque.cloud.
  flows:
  - authorization_code
  how_to_obtain: Register a client via https://bisque.cloud/oauth/register, then follow the authorization code flow to obtain an access token.
  name: OAuth
  scopes:
  - presentations
  - openid
  - email
  type: oauth2
slug: bisque-cloud-authentication
source_filename: bisque-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://bisque.cloud/docs/md/api/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bisque.cloud/docs/md/api/authentication\nsources:\n- https://bisque.cloud/docs/md/api/authentication\n- https://bisque.today/.well-known/oauth-authorization-server\n- https://bisque.cloud/docs/api/authentication\n- https://bisque.today/docs/api/authentication\ndescription: Authentication schemes for Bisque API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Both credentials go in the same header, on every call to the REST API and to the presentations MCP server: Authorization: Bearer\n    <credential>'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth\n  evidence: Bisque is an OAuth 2.1 authorization server with PKCE (S256) and dynamic client registration; the issuer is https://bisque.cloud.\n  flows:\n  - authorization_code\n  authorize_url: https://bisque.cloud/oauth/authorize\n  scopes:\n  - presentations\n  - openid\n  - email\n  how_to_obtain:\
  \ Register a client via https://bisque.cloud/oauth/register, then follow the authorization code flow to obtain an access token.\ndocs: https://bisque.cloud/docs/md/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/bisque-cloud/authentication/bisque-cloud-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Code Presentation
---
