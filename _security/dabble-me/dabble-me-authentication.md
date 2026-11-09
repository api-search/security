---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses OAuth 2.0 with PKCE. The user signs in on Dabble Me’s domain and approves the mcp:access scope.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dabble Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dabble Me declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dabble Me
provider_slug: dabble-me
scheme_count: 1
schemes:
- evidence: OAuth 2.0 + PKCE
  flows:
  - authorization_code
  how_to_obtain: Sign in on Dabble Me’s own domain and approve the mcp:access scope.
  name: OAuth 2.0
  scopes:
  - mcp:access
  type: oauth2
slug: dabble-me-authentication
source_filename: dabble-me-authentication.yml
source_heading: Authentication Profile
source_url: https://dabble.me/mcp-server#agent-instructions
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dabble.me/mcp-server#agent-instructions\nsources:\n- https://dabble.me/mcp-server#agent-instructions\ndescription: Authentication uses OAuth 2.0 with PKCE. The user signs in on Dabble Me’s domain and approves the mcp:access scope.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 + PKCE\n  flows:\n  - authorization_code\n  scopes:\n  - mcp:access\n  how_to_obtain: Sign in on Dabble Me’s own domain and approve the mcp:access scope.\ndocs: https://dabble.me/mcp-server#agent-instructions\n"
source_yaml_url: https://artifacts.apis.io/dabble-me/authentication/dabble-me-authentication.yml
summary_line: 1 scheme
tags:
- Journaling
- Private
- email-first
- AI Integration
- Productivity
---
