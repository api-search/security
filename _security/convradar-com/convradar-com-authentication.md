---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Conversion Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conversion Radar declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Conversion Radar
provider_slug: convradar-com
scheme_count: 1
schemes:
- applies_to: https://mcp.convradar.com/mcp
  discovery: https://mcp.convradar.com/.well-known/oauth-protected-resource
  discovery_standard: RFC 9728
  flow: authorizationCode
  name: OAuth 2.1 (MCP authorization)
  pkce: true
  quote: ConvRadar uses OAuth 2.1 with PKCE. There are no per-user URLs and no manual API key — the client walks the discovery handshake on the protected resource and is redirected to the authorization server on first call.
  scopes:
  - read:metrics
  - write:hypotheses
  token_placement: Bearer token in Authorization header
  type: oauth2
slug: convradar-com-authentication
source_filename: convradar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Conversion Radar authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://convradar.com/docs/mcp\ndocs: https://convradar.com/docs/mcp\nschemes:\n- name: OAuth 2.1 (MCP authorization)\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  token_placement: Bearer token in Authorization header\n  discovery: https://mcp.convradar.com/.well-known/oauth-protected-resource\n  discovery_standard: RFC 9728\n  applies_to: https://mcp.convradar.com/mcp\n  quote: \"ConvRadar uses OAuth 2.1 with PKCE. There are no per-user URLs and no manual API key — the client walks the discovery handshake on the protected resource and is redirected to the authorization server on first call.\"\n  scopes:\n  - read:metrics\n  - write:hypotheses\napi_keys: false\ndownstream_auth: \"The downstream OAuth to Google asks only for read-only GA4 access. ConvRadar cannot modify your analytics data.\"\nnote: No REST/OpenAPI contract is published; authentication described here covers\
  \ the hosted MCP endpoint only.\n"
source_yaml_url: https://artifacts.apis.io/convradar-com/authentication/convradar-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Analytics
- Google Analytics 4
- MCP
- Conversion Rate Optimization
- E-Commerce
- Benchmarks
- AI Agents
---
