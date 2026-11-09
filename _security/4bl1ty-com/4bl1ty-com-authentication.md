---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for the 4bl1ty MCP API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 4Bl1Ty Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: 4bl1ty declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 4bl1ty
provider_slug: 4bl1ty-com
scheme_count: 2
schemes:
- evidence: 'The fastest path is remote: point your client at https://mcp.4bl1ty.com/mcp with an API key and skip every local step.'
  how_to_obtain: Obtain the API key from the 4bl1ty dashboard or account settings.
  name: API key
  type: apiKey
- evidence: Token d'authentification manquant No session in this process. Call auth_login, then auth_status to confirm. The API answers in French — this message means the Authorization header was missing.
  header: Authorization
  how_to_obtain: Call the auth_login tool with email and password to receive a JWT token.
  location: header
  name: Bearer
  type: http-bearer
slug: 4bl1ty-com-authentication
source_filename: 4bl1ty-com-authentication.yml
source_heading: Authentication Profile
source_url: https://4bl1ty.com/mcp/quickstart
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://4bl1ty.com/mcp/quickstart\nsources:\n- https://4bl1ty.com/mcp/quickstart\ndescription: Authentication methods for the 4bl1ty MCP API\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'The fastest path is remote: point your client at https://mcp.4bl1ty.com/mcp with an API key and skip every local step.'\n  how_to_obtain: Obtain the API key from the 4bl1ty dashboard or account settings.\n- type: http-bearer\n  name: Bearer\n  evidence: Token d'authentification manquant No session in this process. Call auth_login, then auth_status to confirm. The API answers in French\n    — this message means the Authorization header was missing.\n  location: header\n  header: Authorization\n  how_to_obtain: Call the auth_login tool with email and password to receive a JWT token.\nnote: No OAuth2 flows, JWT-specific flow, or other authentication schemes are documented on the provided\
  \ pages.\ndocs: https://4bl1ty.com/mcp/quickstart\n"
source_yaml_url: https://artifacts.apis.io/4bl1ty-com/authentication/4bl1ty-com-authentication.yml
summary_line: 2 schemes
tags:
- Marketplace
- Artificial Intelligence
- Human-in-the-Loop
- Task Automation
- France
---
