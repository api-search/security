---
anonymous_access: true
api_key_in: []
auth_types:
- none
- bearer-token
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adordiagnostics Authentication
name_suffix: Authentication
oauth_flows: []
overview: ADOR Diagnostics secures its APIs with none and bearer-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ADOR Diagnostics
provider_slug: adordiagnostics
scheme_count: 2
schemes:
- description: The MCP endpoint https://www.adordx.com/_api/mcp accepts an unauthenticated JSON-RPC tools/list and answers HTTP 200 with 9 tools. tools/call GetBusinessDetails also answers 200 anonymously. No credential is required to connect or to enumerate tools.
  name: anonymous-mcp-connect
  sources:
  - mcp/adordiagnostics-mcp-tools-list.json
  type: none
- description: Tools that act on a visitor's behalf (CallWixSiteAPI, ExecuteWixAPI) require a visitorToken parameter. The token is minted anonymously by the GenerateVisitorToken tool - there is no signup, no API key issuance and no OAuth authorization step. Scope is limited to public site data and visitor-session actions on the Wix apps installed on the site (Blog, Bookings, Ecommerce, Pricing Plans).
  name: visitor-token
  obtained_via: GenerateVisitorToken (MCP tool)
  scheme: bearer
  sources:
  - mcp/adordiagnostics-mcp-tools-list.json
  type: http
slug: adordiagnostics-authentication
source_filename: adordiagnostics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: mcp/adordiagnostics-mcp-tools-list.json\nnote: >-\n  ADOR Diagnostics publishes no OpenAPI and no developer authentication documentation, so there are\n  no securitySchemes to derive from. The only authenticated surface reachable at the adordx.com host\n  is the Wix-provided site MCP endpoint, whose auth model is derived here from its live tools/list\n  response and the anonymous GetBusinessDetails call made on 2026-09-07.\nsummary:\n  types:\n  - none\n  - bearer-token\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: anonymous-mcp-connect\n  type: none\n  description: >-\n    The MCP endpoint https://www.adordx.com/_api/mcp accepts an unauthenticated JSON-RPC tools/list\n    and answers HTTP 200 with 9 tools. tools/call GetBusinessDetails also answers 200 anonymously.\n    No credential is required to connect or to enumerate tools.\n  sources:\n  - mcp/adordiagnostics-mcp-tools-list.json\n- name: visitor-token\n  type:\
  \ http\n  scheme: bearer\n  description: >-\n    Tools that act on a visitor's behalf (CallWixSiteAPI, ExecuteWixAPI) require a visitorToken\n    parameter. The token is minted anonymously by the GenerateVisitorToken tool - there is no\n    signup, no API key issuance and no OAuth authorization step. Scope is limited to public site\n    data and visitor-session actions on the Wix apps installed on the site (Blog, Bookings,\n    Ecommerce, Pricing Plans).\n  obtained_via: GenerateVisitorToken (MCP tool)\n  sources:\n  - mcp/adordiagnostics-mcp-tools-list.json\noauth:\n  present: false\n  evidence: >-\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource returned 400\n    (HTML) on both www.adordx.com and adordx.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adordiagnostics/refs/heads/main/authentication/adordiagnostics-authentication.yml
summary_line: none/bearer-token · 2 schemes
tags:
- Company
- Healthcare
- Medical Devices
- In Vitro Diagnostics
- Molecular Diagnostics
- Infectious Disease
- Point of Care
- Laboratory
- Life Sciences
- MCP
---
