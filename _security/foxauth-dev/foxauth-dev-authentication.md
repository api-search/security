---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foxauth-dev-openapi-generated.yml
  format: yaml
  label: foxauth-dev API
  slug: foxauth-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxauth-dev/openapi/_ae-authored/foxauth-dev-openapi-generated.yml
auth_types: []
description: Client authenticates using HTTP Bearer tokens sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: foxauth-dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: foxauth-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: foxauth-dev
provider_slug: foxauth-dev
scheme_count: 1
schemes:
- evidence: 'When a request arrives with no token, or with a token you reject, you answer 401 and say where your metadata is. This answer is called a challenge: in its WWW-Authenticate header the server tells the client how to get access: HTTP/1.1 401 Unauthorized WWW-Authenticate : Bearer resource_metadata="https://mcp.example.com/.well-known/oauth-protected-resource", scope="mcp:tools-basic"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: foxauth-dev-authentication
source_filename: foxauth-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://foxauth.dev/docs/get-started/protect-your-mcp-server/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://foxauth.dev/docs/get-started/protect-your-mcp-server/\nsources:\n- https://foxauth.dev/docs/get-started/protect-your-mcp-server/\n- https://foxauth.dev/features/\n- https://foxauth.dev/blog/\n- https://foxauth.dev/blog/your-mcp-server-is-an-oauth-resource-server/\ndescription: Client authenticates using HTTP Bearer tokens sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'When a request arrives with no token, or with a token you reject, you answer 401 and say where your metadata is. This answer is called\n    a challenge: in its WWW-Authenticate header the server tells the client how to get access: HTTP/1.1 401 Unauthorized WWW-Authenticate : Bearer\n    resource_metadata=\"https://mcp.example.com/.well-known/oauth-protected-resource\", scope=\"mcp:tools-basic\"'\n  location: header\n  header: Authorization\nnote: No OAuth2 flows\
  \ (client_credentials, authorization_code, etc.) are described on the provided pages.\ndocs: https://foxauth.dev/docs/get-started/protect-your-mcp-server/\n"
source_yaml_url: https://artifacts.apis.io/foxauth-dev/authentication/foxauth-dev-authentication.yml
summary_line: 1 scheme
tags:
- Authorization
- OAuth
- OpenID Connect
- Identity and Access Management
- AI Agents
- MCP
---
