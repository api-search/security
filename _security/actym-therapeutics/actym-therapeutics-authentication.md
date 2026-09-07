---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Actym Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actym Therapeutics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Actym Therapeutics
provider_slug: actym-therapeutics
scheme_count: 2
schemes:
- applies_to:
  - 'MCP: initialize'
  - 'MCP: tools/list'
  - GetBusinessDetails
  - SearchInSite
  - SearchSiteApiDocs
  - BrowseWixRESTDocsMenu
  - ReadFullDocsArticle
  - ReadFullDocsMethodSchema
  evidence: POST https://www.actymthera.com/_api/mcp with no Authorization header returned HTTP 200 and the full tool manifest on 2026-09-06.
  id: anonymous
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  evidence: 'Tool description, verbatim: "Visitor access token. Use GenerateVisitorToken first if not available." GenerateVisitorToken itself declares no parameters.'
  id: wix-visitor-token
  in: tool-parameter
  issued_by: MCP tool GenerateVisitorToken (no credentials required)
  note: This is a visitor session, not an authenticated identity — it grants only what an anonymous browser visitor could do. There is no API key, no OAuth flow, no user account.
  parameter: visitorToken
  type: bearer
slug: actym-therapeutics-authentication
source_filename: actym-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: mcp/actym-therapeutics-tools-list.json\nsummary: >-\n  Actym Therapeutics publishes no API with an authentication scheme. The single callable\n  surface is the anonymous Wix Site MCP endpoint on its own domain, whose auth model is\n  described by the tool manifest itself: discovery (initialize, tools/list) and read tools\n  are anonymous, while the two Wix REST passthrough tools require a short-lived VISITOR\n  token that the same server mints on request.\nschemes:\n- id: anonymous\n  type: none\n  applies_to:\n  - 'MCP: initialize'\n  - 'MCP: tools/list'\n  - GetBusinessDetails\n  - SearchInSite\n  - SearchSiteApiDocs\n  - BrowseWixRESTDocsMenu\n  - ReadFullDocsArticle\n  - ReadFullDocsMethodSchema\n  evidence: >-\n    POST https://www.actymthera.com/_api/mcp with no Authorization header returned HTTP 200\n    and the full tool manifest on 2026-09-06.\n- id: wix-visitor-token\n  type: bearer\n  in: tool-parameter\n  parameter:\
  \ visitorToken\n  issued_by: 'MCP tool GenerateVisitorToken (no credentials required)'\n  applies_to:\n  - CallWixSiteAPI\n  - ExecuteWixAPI\n  evidence: >-\n    Tool description, verbatim: \"Visitor access token. Use GenerateVisitorToken first if not\n    available.\" GenerateVisitorToken itself declares no parameters.\n  note: >-\n    This is a visitor session, not an authenticated identity — it grants only what an\n    anonymous browser visitor could do. There is no API key, no OAuth flow, no user account.\nobserved:\n  http_401:\n    url: https://www.actymthera.com/_api/mcp\n    method: GET\n    status: 401\n    body: '{\"error\":\"invalid_token\",\"error_description\":\"Missing Authorization header\"}'\n    note: The GET surface challenges; the JSON-RPC POST surface used by MCP clients does not.\nabsent:\n  api_keys: true\n  oauth2: true\n  openid_connect: true\n  mutual_tls: true\n  evidence: 'No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (HTTP 400\
  \ on both hosts, 2026-09-06).'\ndocs: null\nnotes:\n- 'No scopes/ artifact is written: there is no OAuth surface, so there is no scope vocabulary to record.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actym-therapeutics/refs/heads/main/authentication/actym-therapeutics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Immuno-Oncology
- Cancer
- Clinical Trials
- Drug Development
- Healthcare
- MCP
---
