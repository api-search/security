---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: The Curator Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Curator declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Curator
provider_slug: curatorapproved-com
scheme_count: 1
schemes:
- applies_to:
  - https://curatorapproved.com/api/mcp
  - https://curatorapproved.com/catalog.json
  description: 'The remote MCP server and the public catalog are unauthenticated. Connect page: "Server URL https://curatorapproved.com/api/mcp Transport Streamable HTTP Authentication None". Connection descriptor (https://curatorapproved.com/connect/mcp.json) declares mcp.authentication.type: none and siteAccess.requiresSitesSignIn: false.'
  name: none
  type: none
slug: curatorapproved-com-authentication
source_filename: curatorapproved-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://curatorapproved.com/connect/\ndocs: https://curatorapproved.com/connect/\nname: The Curator authentication\nschemes:\n- type: none\n  name: none\n  description: 'The remote MCP server and the public catalog are unauthenticated. Connect page: \"Server URL https://curatorapproved.com/api/mcp Transport Streamable HTTP Authentication None\". Connection descriptor (https://curatorapproved.com/connect/mcp.json) declares mcp.authentication.type: none and siteAccess.requiresSitesSignIn: false.'\n  applies_to:\n  - https://curatorapproved.com/api/mcp\n  - https://curatorapproved.com/catalog.json\nnote: 'Browser (WebMCP) saved-finds tools are not credentialed either: they require the visitor to \"Enable browser-agent access\" in the Saved panel of an open tab, scoped to that tab for 15 minutes and 60 operations. llms.txt says owner analytics \"remains protected by Sites\" and delegated analytics is unavailable; no auth mechanism\
  \ for it is documented publicly.'\n"
source_yaml_url: https://artifacts.apis.io/curatorapproved-com/authentication/curatorapproved-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Curation
- Product Discovery
- Music
- Video
- Maker
- MCP
- Catalog
- RSS
---
