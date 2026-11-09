---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Dice Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dice declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dice
provider_slug: dice-com
scheme_count: 1
schemes:
- also_stated:
    quote: Sign-in Not required
    source: https://claude.com/connectors/dice
  client_setup:
    quote: 'Authentication:    Select No Authentication'
    source: https://www.dice.com/career-advice/how-to-connect-the-dice-mcp-server-to-your-ai-assistant
  description: The Dice MCP server is public; no credential is required for basic usage.
  name: anonymous
  quote: This remote MCP server can be accessed directly via its URL. No authentication is required for basic usage.
  type: none
slug: dice-com-authentication
source_filename: dice-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.dice.com/about/mcp\ndocs: https://www.dice.com/about/mcp\napi: dice-com:job-search-mcp\nschemes:\n- type: none\n  name: anonymous\n  description: The Dice MCP server is public; no credential is required for basic usage.\n  quote: \"This remote MCP server can be accessed directly via its URL. No authentication is required for basic usage.\"\n  also_stated:\n    source: https://claude.com/connectors/dice\n    quote: \"Sign-in Not required\"\n  client_setup:\n    source: https://www.dice.com/career-advice/how-to-connect-the-dice-mcp-server-to-your-ai-assistant\n    quote: \"Authentication:    Select No Authentication\"\nnote: Dice publishes no REST/OpenAPI contract and no OAuth, API-key or scopes documentation; the only documented surface is the unauthenticated MCP server at https://mcp.dice.com/mcp. \"basic usage\" implies no authenticated tier is documented.\n"
source_yaml_url: https://artifacts.apis.io/dice-com/authentication/dice-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Job
- Job Search
- Recruiting
- Careers
- Technology Talent
- MCP
---
