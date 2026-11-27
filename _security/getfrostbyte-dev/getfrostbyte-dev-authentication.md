---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Frostbyte MCP API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Frostbyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frostbyte declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Frostbyte
provider_slug: getfrostbyte-dev
scheme_count: 2
schemes:
- evidence: Use dynamic client registration and the authorization-code flow with PKCE S256.
  flows:
  - authorization_code
  how_to_obtain: Dynamic client registration and user authorization via browser (sign‑in, approve, and exchange code).
  name: OAuth2 Authorization Code with PKCE
  scopes:
  - mcp
  - offline_access
  type: oauth2
- evidence: 'Send every MCP request with `Authorization: Bearer <token>`.'
  header: Authorization
  how_to_obtain: User signs in at https://getfrostbyte.dev/login and copies the shown token.
  location: header
  name: Manual token
  type: http-bearer
slug: getfrostbyte-dev-authentication
source_filename: getfrostbyte-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://getfrostbyte.dev/auth.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getfrostbyte.dev/auth.md\nsources:\n- https://getfrostbyte.dev/auth.md\n- https://getfrostbyte.dev/docs/getting-started.md\n- https://getfrostbyte.dev/articles/setup-public-feedback-hub\n- https://getfrostbyte.dev/docs/getting-started\ndescription: Authentication methods for Frostbyte MCP API\nschemes:\n- type: oauth2\n  name: OAuth2 Authorization Code with PKCE\n  evidence: Use dynamic client registration and the authorization-code flow with PKCE S256.\n  flows:\n  - authorization_code\n  scopes:\n  - mcp\n  - offline_access\n  how_to_obtain: Dynamic client registration and user authorization via browser (sign‑in, approve, and exchange code).\n- type: http-bearer\n  name: Manual token\n  evidence: 'Send every MCP request with `Authorization: Bearer <token>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: User signs in at https://getfrostbyte.dev/login and\
  \ copies the shown token.\ndocs: https://getfrostbyte.dev/auth.md\n"
source_yaml_url: https://artifacts.apis.io/getfrostbyte-dev/authentication/getfrostbyte-dev-authentication.yml
summary_line: 2 schemes
tags:
- Software
- Collaboration
- Project Management
- Workspace
- Agents
---
