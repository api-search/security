---
api_key_in: []
auth_types:
- none
- bearer-visitor-token
description: ''
kind: authentication
layout: security
method: searched
name: Kitopi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kitopi secures its APIs with none and bearer-visitor-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kitopi
provider_slug: kitopi
scheme_count: 2
schemes:
- applies_to: https://www.kitopi.com/_api/mcp
  description: No authentication is required to connect to the MCP endpoint or to list and call the read-only tools. Only public site information is exposed.
  name: mcp-anonymous
  source: https://www.kitopi.com/llms.txt
  type: none
- applies_to: CallWixSiteAPI, ExecuteWixAPI
  description: An anonymous visitor access token, minted on demand by the GenerateVisitorToken tool, is required before any call that acts on a visitor's behalf. There is no user account, API key or OAuth client involved; the token represents an unauthenticated site visitor session.
  name: wix-visitor-token
  scheme: bearer
  source: https://www.kitopi.com/llms.txt
  type: http
slug: kitopi-authentication
source_filename: kitopi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.kitopi.com/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nnotes: >-\n  Kitopi publishes no OpenAPI and no developer API, so there are no securitySchemes to derive from.\n  The only reachable programmatic surface is the Wix site MCP endpoint, whose auth model is\n  documented in Kitopi's own llms.txt and verified by live probe: connecting requires no\n  credentials, and acting on a visitor's behalf requires an anonymous visitor token minted by the\n  server itself.\nsummary:\n  types:\n  - none\n  - bearer-visitor-token\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: mcp-anonymous\n  type: none\n  applies_to: https://www.kitopi.com/_api/mcp\n  description: >-\n    No authentication is required to connect to the MCP endpoint or to list and call the read-only\n    tools. Only public site information is exposed.\n  source: https://www.kitopi.com/llms.txt\n\
  - name: wix-visitor-token\n  type: http\n  scheme: bearer\n  applies_to: CallWixSiteAPI, ExecuteWixAPI\n  description: >-\n    An anonymous visitor access token, minted on demand by the GenerateVisitorToken tool, is\n    required before any call that acts on a visitor's behalf. There is no user account, API key or\n    OAuth client involved; the token represents an unauthenticated site visitor session.\n  source: https://www.kitopi.com/llms.txt\nsession:\n  header: mcp-session-id\n  description: >-\n    The MCP server issues an mcp-session-id response header on initialize which must be echoed on\n    subsequent JSON-RPC requests. Observed by live probe on 2026-07-19.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitopi/refs/heads/main/authentication/kitopi-authentication.yml
summary_line: none/bearer-visitor-token · 2 schemes
tags:
- Company
- Consumer
- Food and Beverage
- Cloud Kitchens
- Restaurants
- Food Delivery
- Hospitality
- Middle East
- Logistics
---
