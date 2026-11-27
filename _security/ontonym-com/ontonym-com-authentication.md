---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Ontonym MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ontonym Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ontonym declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ontonym
provider_slug: ontonym-com
scheme_count: 2
schemes:
- evidence: Browser login (OAuth) where supported, or an MCP key
  how_to_obtain: User opens a browser window, signs in to Ontonym and approves access; the minted token appears under Settings → MCP keys and can be revoked there.
  name: Browser login
  type: oauth2
- evidence: 'send it as Authorization: Bearer aio_…'
  header: Authorization
  how_to_obtain: Mint a key in Settings → MCP keys; the key is shown once and used as the Bearer token in the Authorization header.
  location: header
  name: MCP key
  type: http-bearer
slug: ontonym-com-authentication
source_filename: ontonym-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ontonym.com/developers/setup
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ontonym.com/developers/setup\nsources:\n- https://www.ontonym.com/developers/setup\ndescription: Authentication methods for Ontonym MCP\nschemes:\n- type: oauth2\n  name: Browser login\n  evidence: Browser login (OAuth) where supported, or an MCP key\n  how_to_obtain: User opens a browser window, signs in to Ontonym and approves access; the minted token appears under Settings → MCP keys and\n    can be revoked there.\n- type: http-bearer\n  name: MCP key\n  evidence: 'send it as Authorization: Bearer aio_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a key in Settings → MCP keys; the key is shown once and used as the Bearer token in the Authorization header.\ndocs: https://www.ontonym.com/developers/setup\n"
source_yaml_url: https://artifacts.apis.io/ontonym-com/authentication/ontonym-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
