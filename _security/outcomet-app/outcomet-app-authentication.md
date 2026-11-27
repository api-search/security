---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outcomet-app-ask-api-openapi.yml
  format: yaml
  label: Outcomet Ask API
  slug: outcomet-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-ask-api-openapi.yml
- filename: outcomet-app-batch-api-openapi.yml
  format: yaml
  label: Outcomet Batch API
  slug: outcomet-app-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-batch-api-openapi.yml
- filename: outcomet-app-discovery-api-openapi.yml
  format: yaml
  label: Outcomet Discovery API
  slug: outcomet-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-discovery-api-openapi.yml
- filename: outcomet-app-mcp-api-openapi.yml
  format: yaml
  label: Outcomet MCP API
  slug: outcomet-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-mcp-api-openapi.yml
- filename: outcomet-app-onboarding-api-openapi.yml
  format: yaml
  label: Outcomet Onboarding API
  slug: outcomet-app-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-onboarding-api-openapi.yml
- filename: outcomet-app-sandbox-api-openapi.yml
  format: yaml
  label: Outcomet Sandbox API
  slug: outcomet-app-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-sandbox-api-openapi.yml
auth_types: []
description: Outcomet MCP requires OAuth 2.1 Authorization Code flow with PKCE for workspace access; public endpoints are zero‑auth.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Outcomet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Outcomet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Outcomet
provider_slug: outcomet-app
scheme_count: 1
schemes:
- authorize_url: https://mcp.outcomet.app/oauth/authorize
  evidence: Workspace context and tools on the remote Outcomet MCP server (https://mcp.outcomet.app/mcp) require OAuth 2.1 with PKCE (S256) scoped to the signed-in user's Outcomet workspace.
  header: Authorization
  how_to_obtain: Register a public OAuth client dynamically via RFC 7591 at POST https://mcp.outcomet.app/oauth/register, then direct the user to the authorization endpoint with PKCE parameters to obtain an authorization code, and exchange it for an access token at the token endpoint.
  location: header
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - product_context:read
  - feedback:create
  - feedback:write
  - problems:write
  - initiatives:write
  - capabilities:create
  - capabilities:write
  - work_items:write
  - contacts:write
  - competitors:write
  token_url: https://mcp.outcomet.app/oauth/token
  type: http-bearer
slug: outcomet-app-authentication
source_filename: outcomet-app-authentication.yml
source_heading: Authentication Profile
source_url: https://outcomet.app/auth.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://outcomet.app/auth.md\nsources:\n- https://outcomet.app/auth.md\n- https://outcomet.app/.well-known/http-message-signatures-directory\n- https://outcomet.app/developers\n- https://outcomet.app/signup\ndescription: Outcomet MCP requires OAuth 2.1 Authorization Code flow with PKCE for workspace access; public endpoints are zero‑auth.\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: Workspace context and tools on the remote Outcomet MCP server (https://mcp.outcomet.app/mcp) require OAuth 2.1 with PKCE (S256) scoped\n    to the signed-in user's Outcomet workspace.\n  location: header\n  header: Authorization\n  token_url: https://mcp.outcomet.app/oauth/token\n  authorize_url: https://mcp.outcomet.app/oauth/authorize\n  scopes:\n  - product_context:read\n  - feedback:create\n  - feedback:write\n  - problems:write\n  - initiatives:write\n\
  \  - capabilities:create\n  - capabilities:write\n  - work_items:write\n  - contacts:write\n  - competitors:write\n  how_to_obtain: Register a public OAuth client dynamically via RFC 7591 at POST https://mcp.outcomet.app/oauth/register, then direct the user\n    to the authorization endpoint with PKCE parameters to obtain an authorization code, and exchange it for an access token at the token endpoint.\ndocs: https://outcomet.app/auth.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/outcomet-app/authentication/outcomet-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Product Management
- Feedback
- Decision-Making
---
