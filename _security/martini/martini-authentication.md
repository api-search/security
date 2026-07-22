---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Martini Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Martini secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Martini
provider_slug: martini
scheme_count: 1
schemes:
- applies_to: https://www.martini.film/mcp
  flow: authorizationCode
  name: MartiniMCPOAuth
  sources:
  - https://www.martini.film/docs/mcp
  type: oauth2
slug: martini-authentication
source_filename: martini-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.martini.film/docs/mcp\ndocs: https://www.martini.film/security\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  surface: mcp\nnotes: >-\n  Martini has no traditional public REST/OpenAPI surface; its programmatic surface is the\n  hosted MCP connector. Per the MCP docs and /security page, the connector uses OAuth-based\n  authorization where supported: an assistant connects once, the user signs in, and every\n  MCP tool call runs with the same Martini project permissions as the signed-in user.\n  Browser-based MCP requests are restricted to allowed origins. A live GET to the MCP\n  endpoint returns HTTP 401 \"Authentication required\". No API-key scheme is documented.\nschemes:\n- name: MartiniMCPOAuth\n  type: oauth2\n  flow: authorizationCode\n  applies_to: https://www.martini.film/mcp\n  sources: [https://www.martini.film/docs/mcp]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/martini/refs/heads/main/authentication/martini-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video
- Filmmaking
- Generative AI
- Creative Tools
- Model Context Protocol
- Agents
- Collaboration
- Media Production
---
