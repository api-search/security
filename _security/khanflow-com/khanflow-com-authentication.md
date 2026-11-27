---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses OAuth 2.1 Authorization Code flow with PKCE.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Khanflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Khanflow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Khanflow
provider_slug: khanflow-com
scheme_count: 1
schemes:
- evidence: Agents connect through the Khanflow MCP server and OAuth 2.1; there are no API keys to request.
  flows:
  - authorization_code
  how_to_obtain: Register your client at the registration endpoint (https://api.khanflow.com/oauth/register) or use a previously registered client.
  name: OAuth 2.1
  scopes:
  - calendar:read
  - calendar:write
  - tasks:read
  - tasks:write
  - lifeos:read
  - lifeos:write
  - planning
  - availability
  - people:read
  type: oauth2
slug: khanflow-com-authentication
source_filename: khanflow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://khanflow.com/auth.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://khanflow.com/auth.md\nsources:\n- https://khanflow.com/auth.md\ndescription: Authentication uses OAuth 2.1 Authorization Code flow with PKCE.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Agents connect through the Khanflow MCP server and OAuth 2.1; there are no API keys to request.\n  flows:\n  - authorization_code\n  scopes:\n  - calendar:read\n  - calendar:write\n  - tasks:read\n  - tasks:write\n  - lifeos:read\n  - lifeos:write\n  - planning\n  - availability\n  - people:read\n  how_to_obtain: Register your client at the registration endpoint (https://api.khanflow.com/oauth/register) or use a previously registered client.\ndocs: https://khanflow.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/khanflow-com/authentication/khanflow-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Calendar
- Planner
- Productivity
- iOS
---
