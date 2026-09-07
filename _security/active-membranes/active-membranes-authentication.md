---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Active Membranes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Active Membranes declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Active Membranes
provider_slug: active-membranes
scheme_count: 2
schemes:
- applies_to: MCP transport (tools/list, tools/call)
  description: The endpoint accepts anonymous requests. tools/list and tools/call GetBusinessDetails both returned HTTP 200 with no Authorization header and no WWW-Authenticate challenge. There is no OAuth issuer, no RFC 9728 protected resource metadata and no API key of any kind.
  evidence:
    fetched: '2026-09-06'
    http_status: 200
    url: https://www.activemembrane.com/_api/mcp
  id: none
  type: none
- applies_to: CallWixSiteAPI, ExecuteWixAPI
  description: 'Two of the nine tools require a `visitorToken` argument, minted by calling the GenerateVisitorToken tool on the same endpoint. It is an anonymous visitor session for the Wix site, not a customer credential: no signup, account or key issuance is involved, and it grants only what an unauthenticated site visitor can already do. It is issued by the Wix platform, not by Active Membranes.'
  evidence:
    note: inputSchema of CallWixSiteAPI and ExecuteWixAPI both require visitorToken
    url: mcp/active-membranes-mcp-tools.json
  id: wix-visitor-token
  obtained_via: tools/call GenerateVisitorToken
  type: bearer-like session token
slug: active-membranes-authentication
source_filename: active-membranes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  Anonymous JSON-RPC probes of https://www.activemembrane.com/_api/mcp plus the\n  tool input schemas returned by tools/list (saved verbatim at\n  mcp/active-membranes-mcp-tools.json).\nnote: >-\n  There is no OpenAPI to derive from — Active Membranes publishes no REST or\n  GraphQL contract. The only authenticated-adjacent surface is the Wix Site MCP\n  endpoint, and its access model was established by probing it rather than from\n  documentation, because the company documents nothing.\n\nschemes:\n- id: none\n  type: none\n  applies_to: MCP transport (tools/list, tools/call)\n  description: >-\n    The endpoint accepts anonymous requests. tools/list and tools/call\n    GetBusinessDetails both returned HTTP 200 with no Authorization header and no\n    WWW-Authenticate challenge. There is no OAuth issuer, no RFC 9728 protected\n    resource metadata and no API key of any kind.\n  evidence:\n    url: https://www.activemembrane.com/_api/mcp\n\
  \    http_status: 200\n    fetched: '2026-09-06'\n- id: wix-visitor-token\n  type: bearer-like session token\n  applies_to: CallWixSiteAPI, ExecuteWixAPI\n  description: >-\n    Two of the nine tools require a `visitorToken` argument, minted by calling the\n    GenerateVisitorToken tool on the same endpoint. It is an anonymous visitor\n    session for the Wix site, not a customer credential: no signup, account or\n    key issuance is involved, and it grants only what an unauthenticated site\n    visitor can already do. It is issued by the Wix platform, not by\n    Active Membranes.\n  obtained_via: tools/call GenerateVisitorToken\n  evidence:\n    url: mcp/active-membranes-mcp-tools.json\n    note: inputSchema of CallWixSiteAPI and ExecuteWixAPI both require visitorToken\n\nsession_headers_observed:\n- mcp-session-id\n- set-cookie XSRF-TOKEN\n\ndocs: null\ndocs_note: >-\n  Active Membranes publishes no authentication documentation. /developers, /docs\n  and /api all return 404. The only\
  \ provider-published description of the access\n  model is one line in llms.txt: \"No authentication required to connect to the\n  MCP endpoint\".\n\napi_keys: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-membranes/refs/heads/main/authentication/active-membranes-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Water
- Water Technology
- Desalination
- Reverse Osmosis
- Membranes
- Cleantech
- Sustainability
- Industrial
- Hardware
- MCP
- Agents
---
