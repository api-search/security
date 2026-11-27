---
anonymous_access: false
api_key_in: []
api_specs:
- filename: szum-io-openapi-generated.yml
  format: yaml
  label: Szum API
  slug: szum-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/szum-io/openapi/_ae-authored/szum-io-openapi-generated.yml
auth_types: []
description: Authentication methods documented for Szum
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Szum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Szum declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Szum
provider_slug: szum-io
scheme_count: 2
schemes:
- evidence: 'Clients without OAuth support can send an API key as Authorization: Bearer YOUR_API_KEY .'
  header: Authorization
  how_to_obtain: Create and manage keys under Connect → API.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'OAuth is the preferred method for MCP clients that support it: the client opens a browser window, you sign in to Szum, and the client gets scoped access without you pasting an API key into its configuration.'
  how_to_obtain: Sign in to Szum via the OAuth flow; specific URLs are not listed on the page.
  name: MCP OAuth
  type: oauth2
slug: szum-io-authentication
source_filename: szum-io-authentication.yml
source_heading: Authentication Profile
source_url: https://szum.io/docs/authentication
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://szum.io/docs/authentication\nsources:\n- https://szum.io/docs/authentication\n- https://szum.io/docs\n- https://szum.io/docs/editor\ndescription: Authentication methods documented for Szum\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Clients without OAuth support can send an API key as Authorization: Bearer YOUR_API_KEY .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage keys under Connect → API.\n- type: oauth2\n  name: MCP OAuth\n  evidence: 'OAuth is the preferred method for MCP clients that support it: the client opens a browser window, you sign in to Szum, and the client\n    gets scoped access without you pasting an API key into its configuration.'\n  how_to_obtain: Sign in to Szum via the OAuth flow; specific URLs are not listed on the page.\ndocs: https://szum.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/szum-io/authentication/szum-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Visualization
- API
- Charting
- AI Integration
---
