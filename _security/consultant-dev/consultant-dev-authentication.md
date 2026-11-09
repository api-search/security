---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Consultant MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Consultant Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consultant declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Consultant
provider_slug: consultant-dev
scheme_count: 1
schemes:
- authorize_url: https://mcp.consultant.dev/authorize
  evidence: All API tools require OAuth authentication. When you first connect your AI assistant to the MCP server, you will be prompted to sign in with your Consultant account.
  flows:
  - authorization_code
  how_to_obtain: Sign in with your Consultant account when prompted by the AI assistant.
  name: OAuth2
  scopes:
  - openid
  - profile
  - email
  type: oauth2
slug: consultant-dev-authentication
source_filename: consultant-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.consultant.dev/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.consultant.dev/.well-known/oauth-authorization-server\nsources:\n- https://mcp.consultant.dev/.well-known/oauth-authorization-server\n- https://mcp.consultant.dev/.well-known/oauth-protected-resource/mcp\n- https://consultant.dev/mcp/docs\ndescription: Authentication methods for Consultant MCP API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: All API tools require OAuth authentication. When you first connect your AI assistant to the MCP server, you will be prompted to sign\n    in with your Consultant account.\n  flows:\n  - authorization_code\n  authorize_url: https://mcp.consultant.dev/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  how_to_obtain: Sign in with your Consultant account when prompted by the AI assistant.\ndocs: https://mcp.consultant.dev/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/consultant-dev/authentication/consultant-dev-authentication.yml
summary_line: 1 scheme
tags:
- CV Matching
- Contract Assignments
- Rate Calculator
- Income & Tax Tools
- Pension Planner
---
