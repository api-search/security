---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Atomic AGI MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Atomic AGI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Atomic AGI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Atomic AGI
provider_slug: atomicagi-com
scheme_count: 2
schemes:
- evidence: Connect supported AI agents through OAuth 2.1 to call Atomic tools with your existing workspace and project permissions.
  how_to_obtain: Clients with OAuth support open Atomic sign‑in and ask you to approve access. No personal access token is required.
  name: Atomic MCP OAuth
  type: oauth2
- evidence: Create a personal access token only for a client that cannot connect with OAuth.
  header: Authorization
  how_to_obtain: Treat the token like a password; store it in your client config or secret manager.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: atomicagi-com-authentication
source_filename: atomicagi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.atomicagi.com/quickstart.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.atomicagi.com/quickstart.md\nsources:\n- https://docs.atomicagi.com/quickstart.md\n- https://docs.atomicagi.com/settings/profile/mcp.md\ndescription: Authentication methods for Atomic AGI MCP\nschemes:\n- type: oauth2\n  name: Atomic MCP OAuth\n  evidence: Connect supported AI agents through OAuth 2.1 to call Atomic tools with your existing workspace and project permissions.\n  how_to_obtain: Clients with OAuth support open Atomic sign‑in and ask you to approve access. No personal access token is required.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Create a personal access token only for a client that cannot connect with OAuth.\n  location: header\n  header: Authorization\n  how_to_obtain: Treat the token like a password; store it in your client config or secret manager.\ndocs: https://docs.atomicagi.com/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/atomicagi-com/authentication/atomicagi-com-authentication.yml
summary_line: 2 schemes
tags:
- SEO
- Artificial Intelligence
- Analytics
- Marketing
- Search
- Company
---
