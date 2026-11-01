---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Glympt MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Glympt Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: glympt-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: glympt-com
provider_slug: glympt-com
scheme_count: 2
schemes:
- evidence: The hosted endpoint uses OAuth. Leave custom bearer headers empty and follow sign-in.
  how_to_obtain: Sign in to Glympt, select an eligible workspace, and consent through the hosted OAuth flow.
  name: Hosted OAuth
  type: oauth2
- evidence: Create the key in API key settings and provide it as GLYMPT_API_KEY in the adapter’s private process environment.
  header: GLYMPT_API_KEY
  how_to_obtain: Create a scoped key in API key settings of an API‑enabled paid workspace.
  location: header
  name: Local API‑key adapter
  type: apiKey
slug: glympt-com-authentication
source_filename: glympt-com-authentication.yml
source_heading: Authentication Profile
source_url: https://glympt.com/docs/mcp
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://glympt.com/docs/mcp\nsources:\n- https://glympt.com/docs/mcp\ndescription: Authentication methods for Glympt MCP\nschemes:\n- type: oauth2\n  name: Hosted OAuth\n  evidence: The hosted endpoint uses OAuth. Leave custom bearer headers empty and follow sign-in.\n  how_to_obtain: Sign in to Glympt, select an eligible workspace, and consent through the hosted OAuth flow.\n- type: apiKey\n  name: Local API‑key adapter\n  evidence: Create the key in API key settings and provide it as GLYMPT_API_KEY in the adapter’s private process environment.\n  location: header\n  header: GLYMPT_API_KEY\n  how_to_obtain: Create a scoped key in API key settings of an API‑enabled paid workspace.\ndocs: https://glympt.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/glympt-com/authentication/glympt-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Enrichment
- Technographics
- API
- MCP
---
