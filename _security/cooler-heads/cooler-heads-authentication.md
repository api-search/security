---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cooler Heads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cooler Heads declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cooler Heads
provider_slug: cooler-heads
scheme_count: 2
schemes:
- applies_to: https://www.coolerheads.com/_api/mcp
  description: The MCP transport accepts unauthenticated JSON-RPC. initialize, tools/list and the read-only tools (GetBusinessDetails, SearchInSite, SearchSiteApiDocs, the Wix docs readers) all returned 200 with no credential presented.
  evidence: POST tools/list with no Authorization header returned HTTP 200 with 9 tools (probed 2026-08-09)
  name: none
  type: none
- applies_to: https://www.coolerheads.com/_api/mcp
  description: CallWixSiteAPI and ExecuteWixAPI require a visitorToken argument. The token is obtained from the same endpoint by calling GenerateVisitorToken, which itself takes no parameters and no credential — so the token is an anonymous session handle, not an authentication factor. It scopes the caller to the Wix visitor role on this site.
  evidence: tools/list inputSchema for CallWixSiteAPI and ExecuteWixAPI marks visitorToken as required
  issued_by: GenerateVisitorToken tool on https://www.coolerheads.com/_api/mcp
  name: visitorToken
  type: bearer-like session token
slug: cooler-heads-authentication
source_filename: cooler-heads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.coolerheads.com/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nsummary: >-\n  Cooler Heads publishes no developer API and therefore no API key programme, OAuth\n  server or developer credential of any kind. The one callable surface it serves is the\n  anonymous Wix Site MCP endpoint. Connecting to that endpoint requires no\n  authentication at all; acting on a visitor's behalf requires an ephemeral visitor\n  token that any anonymous caller can mint from the endpoint itself via the\n  GenerateVisitorToken tool. There is no user login, no consent step, and no scope\n  model.\nschemes:\n- name: none\n  applies_to: https://www.coolerheads.com/_api/mcp\n  type: none\n  description: >-\n    The MCP transport accepts unauthenticated JSON-RPC. initialize, tools/list and the\n    read-only tools (GetBusinessDetails, SearchInSite, SearchSiteApiDocs, the Wix docs\n \
  \   readers) all returned 200 with no credential presented.\n  evidence: 'POST tools/list with no Authorization header returned HTTP 200 with 9 tools (probed 2026-08-09)'\n- name: visitorToken\n  applies_to: https://www.coolerheads.com/_api/mcp\n  type: bearer-like session token\n  description: >-\n    CallWixSiteAPI and ExecuteWixAPI require a visitorToken argument. The token is\n    obtained from the same endpoint by calling GenerateVisitorToken, which itself takes\n    no parameters and no credential — so the token is an anonymous session handle, not\n    an authentication factor. It scopes the caller to the Wix visitor role on this site.\n  issued_by: GenerateVisitorToken tool on https://www.coolerheads.com/_api/mcp\n  evidence: 'tools/list inputSchema for CallWixSiteAPI and ExecuteWixAPI marks visitorToken as required'\ndiscovery:\n  openid_configuration: absent (HTTP 400)\n  oauth_authorization_server: absent (HTTP 400)\n  oauth_protected_resource: absent (HTTP 400 at host root,\
  \ 404 under /_api/mcp)\nscopes: none published\nabsent:\n- API key programme\n- OAuth 2.0 / OIDC\n- mTLS\n- signed requests\n- developer account or sign-up\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n  - url: https://www.coolerheads.com/llms.txt\n    http_status: 200\n  - url: https://www.coolerheads.com/_api/mcp\n    http_status: 200\n  - url: https://www.coolerheads.com/.well-known/openid-configuration\n    http_status: 400\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooler-heads/refs/heads/main/authentication/cooler-heads-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Oncology
- Scalp Cooling
- Patient Care
- MCP
---
