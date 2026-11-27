---
anonymous_access: true
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Cocktailline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cocktailline secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cocktailline
provider_slug: cocktailline-de
scheme_count: 1
schemes:
- description: The provider's MCP server card declares "authentication":"none"; the server is public and unauthenticated. No API keys, OAuth or other credential schemes are documented.
  evidence: '"transport":"streamable-http","authentication":"none"'
  name: none
  surface: MCP server https://cocktailline.de/mcp (streamable-http)
  type: none
slug: cocktailline-de-authentication
source_filename: cocktailline-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cocktailline.de/.well-known/mcp.json\ndocs: https://cocktailline.de/.well-known/mcp.json\nsummary:\n  types:\n  - none\nschemes:\n- name: none\n  type: none\n  surface: MCP server https://cocktailline.de/mcp (streamable-http)\n  description: The provider's MCP server card declares \"authentication\":\"none\"; the server is public and unauthenticated. No API keys, OAuth or other credential schemes are documented.\n  evidence: '\"transport\":\"streamable-http\",\"authentication\":\"none\"'\n"
source_yaml_url: https://artifacts.apis.io/cocktailline-de/authentication/cocktailline-de-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Cocktails
- Recipes
- Food and Beverage
- Ingredient Finder
- MCP
- Germany
- Consumer
---
