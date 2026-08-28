---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Lunar Outpost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunar Outpost declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lunar Outpost
provider_slug: lunar-outpost
scheme_count: 0
schemes: []
slug: lunar-outpost-authentication
source_filename: lunar-outpost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://www.lunaroutpost.com/_api/mcp\nsummary: >-\n  Lunar Outpost publishes no authenticated developer API, so there is no API key\n  issuance, OAuth client registration or token endpoint to document. The single\n  public machine-readable surface — the site MCP endpoint — requires NO\n  authentication at all. This was established by probe, not from documentation:\n  an anonymous JSON-RPC initialize and tools/list both returned HTTP 200 with no\n  credential presented, and the company's own llms.txt states \"No authentication\n  required to connect to the MCP endpoint\".\n\nschemes: []\n\nsurfaces:\n  - surface: Site MCP endpoint\n    url: https://www.lunaroutpost.com/_api/mcp\n    transport: streamable-http (JSON-RPC 2.0)\n    auth_required: false\n    scheme: none\n    evidence:\n      - probe: 'POST tools/list with no Authorization header'\n        http_status: 200\n      - probe: 'POST initialize with no Authorization header'\n\
  \        http_status: 200\n      - probe: 'GET with no Authorization header'\n        http_status: 401\n        note: >-\n          Returns {\"error\":\"invalid_token\"}. This is a METHOD artefact, not an auth\n          requirement — the same URL answers an anonymous POST with 200. Do not read\n          this 401 as a credential gate.\n      - source: https://www.lunaroutpost.com/llms.txt\n        quote: 'No authentication required to connect to the MCP endpoint'\n    notes: >-\n      A per-session visitor token exists but it is NOT a credential a caller must\n      obtain out of band — the endpoint mints it anonymously via the\n      GenerateVisitorToken tool, and it is required only for the two mutating tools\n      (CallWixSiteAPI, ExecuteWixAPI). The server also sets an XSRF-TOKEN cookie and\n      returns an mcp-session-id header. Access is limited by scope, not by identity:\n      only public site information is reachable.\n\noauth_discovery:\n  probed: true\n  results:\n    - url:\
  \ https://www.lunaroutpost.com/.well-known/oauth-authorization-server\n      status: 400\n    - url: https://www.lunaroutpost.com/.well-known/oauth-protected-resource\n      status: 400\n    - url: https://www.lunaroutpost.com/.well-known/openid-configuration\n      status: 400\n  note: >-\n    All three return the Wix catch-all 400 error page, byte-identical to a control\n    probe of a nonexistent path. No OAuth or OIDC discovery metadata is served.\n\nscopes: none\nmutual_tls: false\napi_keys: false\n\ngaps:\n  - >-\n    Lunar Outpost's actual mission-operations products (Stargate, Starweave, Spark)\n    are operated under government and defence contract and expose no public\n    authentication surface. Nothing here describes access to those systems.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-outpost/refs/heads/main/authentication/lunar-outpost-authentication.yml
summary_line: 0 schemes
tags:
- Space
- Robotics
- Aerospace
- Lunar Exploration
- Autonomous Systems
- Mission Control
- Defense
- Satellite
- Artificial Intelligence
- Company
---
