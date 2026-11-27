---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for BriefMe MCP endpoints
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BriefMe Authentication
name_suffix: Authentication
oauth_flows: []
overview: BriefMe declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BriefMe
provider_slug: briefme-us
scheme_count: 2
schemes:
- evidence: Authentication None required (OAuth 2.0 optional, to link a BriefMe account)
  name: None
  type: other
- evidence: Both authenticate with OAuth 2.0 (dynamic client registration, PKCE).
  how_to_obtain: dynamic client registration, PKCE
  name: OAuth 2.0
  type: oauth2
slug: briefme-us-authentication
source_filename: briefme-us-authentication.yml
source_heading: Authentication Profile
source_url: https://briefme.us/docs/mcp
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://briefme.us/docs/mcp\nsources:\n- https://briefme.us/docs/mcp\ndescription: Authentication methods for BriefMe MCP endpoints\nschemes:\n- type: other\n  name: None\n  evidence: Authentication None required (OAuth 2.0 optional, to link a BriefMe account)\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Both authenticate with OAuth 2.0 (dynamic client registration, PKCE).\n  how_to_obtain: dynamic client registration, PKCE\ndocs: https://briefme.us/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/briefme-us/authentication/briefme-us-authentication.yml
summary_line: 2 schemes
tags:
- Timer
- Meetings
- Productivity
- Software-as-a-Service
- Free
---
