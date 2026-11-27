---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for KrystalView MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: KrystalView Authentication
name_suffix: Authentication
oauth_flows: []
overview: KrystalView declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: KrystalView
provider_slug: krystalview-com
scheme_count: 2
schemes:
- evidence: Remote clients should use OAuth authorization code with PKCE.
  flows:
  - authorization_code
  how_to_obtain: Use the OAuth authorization code flow with PKCE as described in the MCP documentation.
  name: OAuth
  type: oauth2
- evidence: 'Clients that support custom headers can call the hosted endpoint with a KrystalView read API key as Authorization: Bearer kv_live_... or X-API-Key: kv_live_....'
  header: Authorization
  how_to_obtain: Set the KRYSTALVIEW_API_KEY environment variable to a site‑scoped read‑only API key.
  location: header
  name: API Key
  type: apiKey
slug: krystalview-com-authentication
source_filename: krystalview-com-authentication.yml
source_heading: Authentication Profile
source_url: https://krystalview.com/docs/mcp
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://krystalview.com/docs/mcp\nsources:\n- https://krystalview.com/docs/mcp\ndescription: Authentication methods for KrystalView MCP\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Remote clients should use OAuth authorization code with PKCE.\n  flows:\n  - authorization_code\n  how_to_obtain: Use the OAuth authorization code flow with PKCE as described in the MCP documentation.\n- type: apiKey\n  name: API Key\n  evidence: 'Clients that support custom headers can call the hosted endpoint with a KrystalView read API key as Authorization: Bearer kv_live_...\n    or X-API-Key: kv_live_....'\n  location: header\n  header: Authorization\n  how_to_obtain: Set the KRYSTALVIEW_API_KEY environment variable to a site‑scoped read‑only API key.\ndocs: https://krystalview.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/krystalview-com/authentication/krystalview-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Analytics
- Web
- Mobile
- Data
---
