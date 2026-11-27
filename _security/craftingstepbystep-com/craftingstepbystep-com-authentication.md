---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Crafting Step by Step Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crafting Step by Step declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Crafting Step by Step
provider_slug: craftingstepbystep-com
scheme_count: 2
schemes:
- applies_to: MCP server https://www.craftingstepbystep.com/api/mcp
  evidence: '"Endpoint: https://www.craftingstepbystep.com/api/mcp (streamable HTTP, no auth)" (llms.txt); mcp.json transports[0].authentication.type = none (https://www.craftingstepbystep.com/.well-known/mcp.json)'
  type: none
- applies_to: Citation endpoint https://www.craftingstepbystep.com/api/citation/{slug}
  evidence: Unauthenticated HEAD of /api/citation/how-to-knit-a-sweater returned HTTP 200 application/json on 2026-11-04 (probed); llms.txt documents the endpoint with no credential requirement.
  type: none
slug: craftingstepbystep-com-authentication
source_filename: craftingstepbystep-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.craftingstepbystep.com/llms.txt\ndocs: https://www.craftingstepbystep.com/llms.txt\nschemes:\n- type: none\n  applies_to: MCP server https://www.craftingstepbystep.com/api/mcp\n  evidence: '\"Endpoint: https://www.craftingstepbystep.com/api/mcp (streamable HTTP, no auth)\" (llms.txt); mcp.json transports[0].authentication.type = none (https://www.craftingstepbystep.com/.well-known/mcp.json)'\n- type: none\n  applies_to: Citation endpoint https://www.craftingstepbystep.com/api/citation/{slug}\n  evidence: Unauthenticated HEAD of /api/citation/how-to-knit-a-sweater returned HTTP 200 application/json on 2026-11-04 (probed); llms.txt documents the endpoint with no credential requirement.\nnote: No API keys, OAuth or scopes are documented anywhere; the provider publishes no developer portal (/developers and /api return 404).\n"
source_yaml_url: https://artifacts.apis.io/craftingstepbystep-com/authentication/craftingstepbystep-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Crafts
- Tutorials
- How-To
- DIY
- Education
- MCP
---
