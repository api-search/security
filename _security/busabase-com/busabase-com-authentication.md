---
anonymous_access: false
api_key_in: []
api_specs:
- filename: busabase-com-openapi.json
  format: json
  label: Busabase API
  slug: busabase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busabase-com/openapi/busabase-com-openapi.json
auth_types: []
description: Authentication methods for Busabase
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Busabase Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: busabase-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: busabase-com
provider_slug: busabase-com
scheme_count: 2
schemes:
- evidence: On Busabase Cloud, the client opens a browser-based OAuth flow where you choose the Busabase account, permission level, and expiration.
  flows:
  - authorization_code
  how_to_obtain: The client opens a browser window, signs in, reviews the requested mcp scope, and authorizes the grant. No client secret is required.
  name: MCP OAuth
  type: oauth2
- evidence: 'Put the key in the Authorization header:'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys, then use it as a Bearer token in the Authorization header.
  location: header
  name: API Key
  type: http-bearer
slug: busabase-com-authentication
source_filename: busabase-com-authentication.yml
source_heading: Authentication Profile
source_url: https://busabase.com/docs/mcp
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://busabase.com/docs/mcp\nsources:\n- https://busabase.com/docs/mcp\n- https://busabase.com/docs/api-keys\n- https://busabase.com/docs/rest-api\n- https://busabase.com/SETUP_SKILL.md\ndescription: Authentication methods for Busabase\nschemes:\n- type: oauth2\n  name: MCP OAuth\n  evidence: On Busabase Cloud, the client opens a browser-based OAuth flow where you choose the Busabase account, permission level, and expiration.\n  flows:\n  - authorization_code\n  how_to_obtain: The client opens a browser window, signs in, reviews the requested mcp scope, and authorizes the grant. No client secret is required.\n- type: http-bearer\n  name: API Key\n  evidence: 'Put the key in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys, then use it as a Bearer token in the Authorization header.\ndocs: https://busabase.com/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/busabase-com/authentication/busabase-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Workspace
- Open Source
- Cloud
- Self-Hosted
---
