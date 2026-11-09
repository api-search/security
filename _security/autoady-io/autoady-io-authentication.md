---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for AutoAdy API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Autoady Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoAdy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AutoAdy
provider_slug: autoady-io
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer adk_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create a key in Settings → AI & Agents → AutoAdy API keys and copy the full `adk_` key.
  location: header
  name: AutoAdy API key
  type: http-bearer
- evidence: Clients that implement MCP authorization can sign in and approve AutoAdy through OAuth 2.1.
  how_to_obtain: Use the remote MCP endpoint; a manual key is not needed for that flow.
  name: Remote MCP OAuth
  type: oauth2
slug: autoady-io-authentication
source_filename: autoady-io-authentication.yml
source_heading: Authentication Profile
source_url: https://help.autoady.io/agent/ai-providers.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.autoady.io/agent/ai-providers.md\nsources:\n- https://help.autoady.io/agent/ai-providers.md\n- https://help.autoady.io/developers/authentication.md\n- https://help.autoady.io/developers/authentication\n- https://help.autoady.io/quickstart.md\ndescription: Authentication methods for AutoAdy API\nschemes:\n- type: http-bearer\n  name: AutoAdy API key\n  evidence: 'Authorization: Bearer adk_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → AI & Agents → AutoAdy API keys and copy the full `adk_` key.\n- type: oauth2\n  name: Remote MCP OAuth\n  evidence: Clients that implement MCP authorization can sign in and approve AutoAdy through OAuth 2.1.\n  how_to_obtain: Use the remote MCP endpoint; a manual key is not needed for that flow.\ndocs: https://help.autoady.io/agent/ai-providers.md\n"
source_yaml_url: https://artifacts.apis.io/autoady-io/authentication/autoady-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Advertising
- Media Buying
- Marketing
---
