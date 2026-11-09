---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Find Codes Authentication
name_suffix: Authentication
oauth_flows: []
overview: find.codes declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: find.codes
provider_slug: find-codes
scheme_count: 1
schemes:
- description: 'The find.codes MCP endpoint (POST https://find.codes/api/mcp) and the plain JSON catalog (GET https://find.codes/codes.json) are served publicly without any API key, token or session. The HTTP 405 body returned by GET /api/mcp states: "This MCP server is stateless: send JSON-RPC 2.0 messages via POST. See https://find.codes/codes.json for the plain-JSON catalog." No authentication, OAuth, API-key or sign-up page is documented on the site. The provider publishes an llms.txt (https://find.codes/llms.txt) and a Content-Signal response header advertising that AI agents may read and train on the data.'
  type: none
slug: find-codes-authentication
source_filename: find-codes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://find.codes/api/mcp\nname: find.codes authentication\nschemes:\n  - type: none\n    description: >-\n      The find.codes MCP endpoint (POST https://find.codes/api/mcp) and the\n      plain JSON catalog (GET https://find.codes/codes.json) are served publicly\n      without any API key, token or session. The HTTP 405 body returned by GET\n      /api/mcp states: \"This MCP server is stateless: send JSON-RPC 2.0 messages\n      via POST. See https://find.codes/codes.json for the plain-JSON catalog.\"\n      No authentication, OAuth, API-key or sign-up page is documented on the\n      site. The provider publishes an llms.txt (https://find.codes/llms.txt) and\n      a Content-Signal response header advertising that AI agents may read and\n      train on the data.\nnotes: >-\n  Access is unauthenticated and read-only. Affiliate referral/discount codes\n  returned by the service are not credentials to find.codes itself.\n"
source_yaml_url: https://artifacts.apis.io/find-codes/authentication/find-codes-authentication.yml
summary_line: 1 scheme
tags:
- Promo Codes
- Referral Codes
- Discount Codes
- Affiliate
- Cryptocurrency
- Exchanges
- Travel eSIM
- MCP
---
