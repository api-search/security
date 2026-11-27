---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CourtlyGo Authentication
name_suffix: Authentication
oauth_flows: []
overview: CourtlyGo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CourtlyGo
provider_slug: courtlygo-com
scheme_count: 1
schemes:
- applies_to:
  - https://courtlygo.com/mcp
  - https://courtlygo.com/data
  evidence: The CourtlyGo MCP server is open (no key or sign-in) and read-only
  type: none
slug: courtlygo-com-authentication
source_filename: courtlygo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://courtlygo.com/developers\ndocs: https://courtlygo.com/developers\nsummary: No authentication. The developers page states the MCP server \"is open (no key or sign-in) and read-only\"; the city data files are plain public JSON downloads. No OpenAPI contract is published.\nschemes:\n- type: none\n  applies_to: [https://courtlygo.com/mcp, https://courtlygo.com/data]\n  evidence: The CourtlyGo MCP server is open (no key or sign-in) and read-only\n"
source_yaml_url: https://artifacts.apis.io/courtlygo-com/authentication/courtlygo-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sports
- Tennis
- Pickleball
- Padel
- Open Data
- OpenStreetMap
- MCP
- AI Agents
- Geolocation
---
