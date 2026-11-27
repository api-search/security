---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods described on the MCP page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FreeVideoGenerator Authentication
name_suffix: Authentication
oauth_flows: []
overview: FreeVideoGenerator declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FreeVideoGenerator
provider_slug: freevideogenerator-app
scheme_count: 2
schemes:
- evidence: Do I need an API key? No API key is needed when your client supports browser-based OAuth.
  name: OAuth 2.1
  type: oauth2
- evidence: MCP API keys are available for clients that need them.
  name: MCP API Key
  type: apiKey
slug: freevideogenerator-app-authentication
source_filename: freevideogenerator-app-authentication.yml
source_heading: Authentication Profile
source_url: https://freevideogenerator.app/mcp
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://freevideogenerator.app/mcp\nsources:\n- https://freevideogenerator.app/mcp\ndescription: Authentication methods described on the MCP page.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Do I need an API key? No API key is needed when your client supports browser-based OAuth.\n- type: apiKey\n  name: MCP API Key\n  evidence: MCP API keys are available for clients that need them.\ndocs: https://freevideogenerator.app/mcp\n"
source_yaml_url: https://artifacts.apis.io/freevideogenerator-app/authentication/freevideogenerator-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Video
- Generation
- FreeCredits
- Creator Tools
---
