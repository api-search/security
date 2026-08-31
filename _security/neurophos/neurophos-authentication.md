---
api_key_in: []
auth_types:
- none
- bearer-token
description: ''
kind: authentication
layout: security
method: derived
name: Neurophos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neurophos secures its APIs with none and bearer-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Neurophos
provider_slug: neurophos
scheme_count: 2
schemes:
- description: The MCP endpoint https://www.neurophos.com/_api/mcp accepts an unauthenticated JSON-RPC tools/list and answers 200. No credential is required to connect or to enumerate tools.
  name: anonymous-mcp-connect
  sources:
  - mcp/neurophos-mcp-tools-list.json
  type: none
- description: Tools that act on a visitor's behalf (CallWixSiteAPI, ExecuteWixAPI) require a visitorToken parameter. The token is minted anonymously by the GenerateVisitorToken tool — there is no signup, no API key issuance, and no OAuth authorization step. Scope is limited to public site data and visitor-session actions.
  name: visitor-token
  obtained_via: GenerateVisitorToken (MCP tool)
  scheme: bearer
  sources:
  - mcp/neurophos-mcp-tools-list.json
  type: http
slug: neurophos-authentication
source_filename: neurophos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: mcp/neurophos-mcp-tools-list.json\nnote: >-\n  Neurophos publishes no OpenAPI and no developer authentication documentation, so there\n  are no securitySchemes to derive from. The only authenticated surface reachable at the\n  neurophos.com host is the Wix-provided site MCP endpoint, whose auth model is derived\n  here from its live tools/list response.\nsummary:\n  types:\n  - none\n  - bearer-token\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: anonymous-mcp-connect\n  type: none\n  description: >-\n    The MCP endpoint https://www.neurophos.com/_api/mcp accepts an unauthenticated\n    JSON-RPC tools/list and answers 200. No credential is required to connect or to\n    enumerate tools.\n  sources:\n  - mcp/neurophos-mcp-tools-list.json\n- name: visitor-token\n  type: http\n  scheme: bearer\n  description: >-\n    Tools that act on a visitor's behalf (CallWixSiteAPI, ExecuteWixAPI) require a\n    visitorToken parameter.\
  \ The token is minted anonymously by the GenerateVisitorToken\n    tool — there is no signup, no API key issuance, and no OAuth authorization step.\n    Scope is limited to public site data and visitor-session actions.\n  obtained_via: GenerateVisitorToken (MCP tool)\n  sources:\n  - mcp/neurophos-mcp-tools-list.json\noauth:\n  present: false\n  evidence: /.well-known/oauth-authorization-server returned 400 (site) and 404 (MCP path)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurophos/refs/heads/main/authentication/neurophos-authentication.yml
summary_line: none/bearer-token · 2 schemes
tags:
- Company
- photonics
- Optical Computing
- ai-inference
- ai-accelerators
- semiconductors
- Metamaterials
- data-center
- deep-tech
- MCP
---
