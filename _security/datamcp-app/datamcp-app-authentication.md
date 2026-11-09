---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datamcp-app-openapi-generated.yml
  format: yaml
  label: datamcp API
  slug: datamcp-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datamcp-app/openapi/_ae-authored/datamcp-app-openapi-generated.yml
auth_types: []
description: Authentication schemes supported by DataMCP as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Datamcp App Authentication
name_suffix: Authentication
oauth_flows: []
overview: datamcp declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: datamcp
provider_slug: datamcp-app
scheme_count: 6
schemes:
- evidence: "components:\n  securitySchemes:\n    ApiKeyAuth:\n      type: apiKey\n      in: header\n      name: X-API-Key"
  header: X-API-Key
  location: header
  name: ApiKeyAuth
  type: apiKey
- evidence: 'Header: X-API-Key: secret

    Query: ?api_key=secret

    Cookie: Cookie: session_key=secret'
  header: api_key
  location: query
  name: ApiKeyAuthQuery
  type: apiKey
- evidence: 'Header: X-API-Key: secret

    Query: ?api_key=secret

    Cookie: Cookie: session_key=secret'
  header: session_key
  location: cookie
  name: ApiKeyAuthCookie
  type: apiKey
- evidence: 'Bearer authentication sends a token in the HTTP authorization header:

    Authorization: Bearer YOUR_TOKEN'
  header: Authorization
  location: header
  name: BearerAuth
  type: http-bearer
- evidence: 'HTTP Basic combines a username and password and sends the Base64-encoded result in the authorization header:

    Authorization: Basic BASE64_USERNAME_AND_PASSWORD'
  header: Authorization
  location: header
  name: BasicAuth
  type: http-basic
- evidence: data mcp supports OAuth 2.0 with PKCE for the client-to-MCP boundary.
  name: OAuth2PKCE
  type: oauth2
slug: datamcp-app-authentication
source_filename: datamcp-app-authentication.yml
source_heading: Authentication Profile
source_url: https://datamcp.app/blog/openapi-authentication-for-mcp
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datamcp.app/blog/openapi-authentication-for-mcp\nsources:\n- https://datamcp.app/blog/openapi-authentication-for-mcp\n- https://datamcp.app/docs/zapier\n- https://datamcp.app/blog/chatgpt-mcp-setup-guide\n- https://datamcp.app/blog/claude-code-mcp-setup\ndescription: Authentication schemes supported by DataMCP as described on the documentation pages.\nschemes:\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: \"components:\\n  securitySchemes:\\n    ApiKeyAuth:\\n      type: apiKey\\n      in: header\\n      name: X-API-Key\"\n  location: header\n  header: X-API-Key\n- type: apiKey\n  name: ApiKeyAuthQuery\n  evidence: 'Header: X-API-Key: secret\n\n    Query: ?api_key=secret\n\n    Cookie: Cookie: session_key=secret'\n  location: query\n  header: api_key\n- type: apiKey\n  name: ApiKeyAuthCookie\n  evidence: 'Header: X-API-Key: secret\n\n    Query: ?api_key=secret\n\n   \
  \ Cookie: Cookie: session_key=secret'\n  location: cookie\n  header: session_key\n- type: http-bearer\n  name: BearerAuth\n  evidence: 'Bearer authentication sends a token in the HTTP authorization header:\n\n    Authorization: Bearer YOUR_TOKEN'\n  location: header\n  header: Authorization\n- type: http-basic\n  name: BasicAuth\n  evidence: 'HTTP Basic combines a username and password and sends the Base64-encoded result in the authorization header:\n\n    Authorization: Basic BASE64_USERNAME_AND_PASSWORD'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth2PKCE\n  evidence: data mcp supports OAuth 2.0 with PKCE for the client-to-MCP boundary.\ndocs: https://datamcp.app/blog/openapi-authentication-for-mcp\n"
source_yaml_url: https://artifacts.apis.io/datamcp-app/authentication/datamcp-app-authentication.yml
summary_line: 6 schemes
tags:
- Database
- MCP
- OpenAPI
- Artificial Intelligence
---
