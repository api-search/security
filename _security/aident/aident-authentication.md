---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses Aident's OAuth flow discovered automatically by the MCP client.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aident Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aident Loadout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aident Loadout
provider_slug: aident
scheme_count: 1
schemes:
- evidence: 'On first use, your MCP client will automatically:

    1. Discover Aident''s OAuth endpoints

    2. Open your browser for login (Google OAuth or magic link)

    3. Store your access token locally'
  how_to_obtain: The MCP client discovers the OAuth endpoints, opens a browser for the user to sign in, and stores the access token locally.
  name: Aident OAuth
  type: oauth2
slug: aident-authentication
source_filename: aident-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.aident.ai/loadout/setup-agents.md
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.aident.ai/loadout/setup-agents.md\nsources:\n- https://docs.aident.ai/loadout/setup-agents.md\n- https://docs.aident.ai/documentation/mcp-server-setup.md\ndescription: Authentication uses Aident's OAuth flow discovered automatically by the MCP client.\nschemes:\n- type: oauth2\n  name: Aident OAuth\n  evidence: 'On first use, your MCP client will automatically:\n\n    1. Discover Aident''s OAuth endpoints\n\n    2. Open your browser for login (Google OAuth or magic link)\n\n    3. Store your access token locally'\n  how_to_obtain: The MCP client discovers the OAuth endpoints, opens a browser for the user to sign in, and stores the access token locally.\ndocs: https://docs.aident.ai/loadout/setup-agents.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aident/refs/heads/main/authentication/aident-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Integration
- Automation
- Platform
---
