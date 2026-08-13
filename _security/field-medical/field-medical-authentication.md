---
api_key_in: []
auth_types:
- none
- bearer-visitor-token
description: ''
kind: authentication
layout: security
method: probed
name: Field Medical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Field Medical secures its APIs with none and bearer-visitor-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Field Medical
provider_slug: field-medical
scheme_count: 2
schemes:
- applies_to:
  - tools/list
  - initialize
  - GetBusinessDetails
  - SearchInSite
  - SearchSiteApiDocs
  evidence: POST https://www.fieldmedicalinc.com/_api/mcp with no credentials returned HTTP 200 and the full nine-tool manifest on 2026-08-12.
  name: anonymous-jsonrpc
  sources:
  - mcp/field-medical-mcp-tools.json
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  evidence: 'visitorToken is a required inputSchema property on CallWixSiteAPI and ExecuteWixAPI in the live tools/list response; the published tool description states: "You must use this tool before calling CallWixSiteAPI".'
  name: wix-visitor-token
  obtained_via: GenerateVisitorToken (MCP tool, no credentials required)
  scheme: bearer
  sources:
  - mcp/field-medical-mcp-tools.json
  - llms/field-medical-llms.txt
  type: http
slug: field-medical-authentication
source_filename: field-medical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.fieldmedicalinc.com/_api/mcp\nscope: Applies ONLY to the Wix-provided site MCP endpoint served at Field Medical's\n  domain. Field Medical publishes no developer portal, no REST/GraphQL API and no\n  authentication documentation of its own; there is no OpenAPI in this repo to derive\n  securitySchemes from. Everything below was observed live, not read from a provider\n  auth page.\nsummary:\n  types:\n  - none\n  - bearer-visitor-token\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: anonymous-jsonrpc\n  type: none\n  applies_to:\n  - tools/list\n  - initialize\n  - GetBusinessDetails\n  - SearchInSite\n  - SearchSiteApiDocs\n  evidence: POST https://www.fieldmedicalinc.com/_api/mcp with no credentials returned\n    HTTP 200 and the full nine-tool manifest on 2026-08-12.\n  sources:\n  - mcp/field-medical-mcp-tools.json\n- name: wix-visitor-token\n  type: http\n  scheme: bearer\n  applies_to:\n  - CallWixSiteAPI\n\
  \  - ExecuteWixAPI\n  obtained_via: GenerateVisitorToken (MCP tool, no credentials required)\n  evidence: 'visitorToken is a required inputSchema property on CallWixSiteAPI and\n    ExecuteWixAPI in the live tools/list response; the published tool description states:\n    \"You must use this tool before calling CallWixSiteAPI\".'\n  sources:\n  - mcp/field-medical-mcp-tools.json\n  - llms/field-medical-llms.txt\nnotes:\n- A plain GET on https://www.fieldmedicalinc.com/_api/mcp returns HTTP 401; the endpoint\n  answers JSON-RPC POST only.\n- No OAuth 2.0 / OIDC discovery is served — /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/openid-configuration all\n  returned HTTP 400 HTML (see well-known/field-medical-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/field-medical/refs/heads/main/authentication/field-medical-authentication.yml
summary_line: none/bearer-visitor-token · 2 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Medical Technology
- Clinical Research
- Model Context Protocol
---
