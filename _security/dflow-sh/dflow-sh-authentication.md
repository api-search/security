---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for dFlow MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: dFlow Authentication
name_suffix: Authentication
oauth_flows: []
overview: dFlow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: dFlow
provider_slug: dflow-sh
scheme_count: 1
schemes:
- authorize_url: https://app.dflow.sh/oauth/authorize
  evidence: 'Agents use the MCP OAuth 2.0 stack on the dashboard:'
  how_to_obtain: Register a public OAuth client at https://app.dflow.sh/api/oauth/register, then have a user authorize at https://app.dflow.sh/oauth/authorize to obtain an authorization code, exchange it for an access token, and use the token as a Bearer token in the Authorization header.
  name: OAuth 2.0 Authorization Code with PKCE
  scopes:
  - mcp
  token_url: https://app.dflow.sh/api/oauth/token
  type: oauth2
slug: dflow-sh-authentication
source_filename: dflow-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://dflow.sh/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dflow.sh/.well-known/oauth-authorization-server\nsources:\n- https://dflow.sh/.well-known/oauth-authorization-server\n- https://dflow.sh/auth.md\ndescription: Authentication for dFlow MCP API\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Authorization Code with PKCE\n  evidence: 'Agents use the MCP OAuth 2.0 stack on the dashboard:'\n  token_url: https://app.dflow.sh/api/oauth/token\n  authorize_url: https://app.dflow.sh/oauth/authorize\n  scopes:\n  - mcp\n  how_to_obtain: Register a public OAuth client at https://app.dflow.sh/api/oauth/register, then have a user authorize at https://app.dflow.sh/oauth/authorize\n    to obtain an authorization code, exchange it for an access token, and use the token as a Bearer token in the Authorization header.\ndocs: https://dflow.sh/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/dflow-sh/authentication/dflow-sh-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Infrastructure
- Platform
- Deployment
- Automation
---
