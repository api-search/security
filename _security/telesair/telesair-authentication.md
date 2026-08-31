---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Telesair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telesair declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Telesair
provider_slug: telesair
scheme_count: 2
schemes:
- applies_to:
  - initialize
  - tools/list
  - GetBusinessDetails
  - SearchInSite
  - SearchSiteApiDocs
  - BrowseWixRESTDocsMenu
  - ReadFullDocsArticle
  - ReadFullDocsMethodSchema
  evidence: POST initialize and POST tools/list both returned HTTP 200 with no Authorization header and no OAuth challenge, probed 2026-08-30.
  id: mcp-anonymous
  surface: https://www.telesair.com/_api/mcp
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  evidence: The GenerateVisitorToken tool mints an anonymous visitor session token with no credential; both write-capable tools declare visitorToken as a required inputSchema property.
  id: wix-visitor-token
  in: tool-parameter
  issuance: self-service
  issuance_tool: GenerateVisitorToken
  parameter: visitorToken
  scheme: bearer
  surface: https://www.telesair.com/_api/mcp
  type: http
slug: telesair-authentication
source_filename: telesair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://www.telesair.com/_api/mcp (live MCP initialize + tools/list)\nsummary: >-\n  Telesair publishes no REST/GraphQL API and therefore declares no securitySchemes anywhere. The\n  only authenticated surface it exposes is the Wix Site Visitor Assistant MCP endpoint served from\n  its own host, whose auth model was established by live probe rather than from documentation.\nschemes:\n- id: mcp-anonymous\n  surface: https://www.telesair.com/_api/mcp\n  type: none\n  applies_to: [initialize, tools/list, GetBusinessDetails, SearchInSite, SearchSiteApiDocs, BrowseWixRESTDocsMenu, ReadFullDocsArticle, ReadFullDocsMethodSchema]\n  evidence: >-\n    POST initialize and POST tools/list both returned HTTP 200 with no Authorization header and no\n    OAuth challenge, probed 2026-08-30.\n- id: wix-visitor-token\n  surface: https://www.telesair.com/_api/mcp\n  type: http\n  scheme: bearer\n  in: tool-parameter\n  parameter: visitorToken\n\
  \  applies_to: [CallWixSiteAPI, ExecuteWixAPI]\n  issuance: self-service\n  issuance_tool: GenerateVisitorToken\n  evidence: >-\n    The GenerateVisitorToken tool mints an anonymous visitor session token with no credential; both\n    write-capable tools declare visitorToken as a required inputSchema property.\noauth: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nscopes: null\nscopes_note: >-\n  No OAuth surface exists, so no scopes/ artifact is emitted. /.well-known/oauth-authorization-server\n  and /.well-known/oauth-protected-resource both returned HTTP 400 (Wix catch-all).\ndocs: null\ndocs_note: >-\n  Telesair publishes no authentication documentation of any kind; this profile is derived entirely\n  from the live MCP handshake.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telesair/refs/heads/main/authentication/telesair-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Medical Devices
- Healthcare
- Respiratory Care
- MedTech
- Hardware
- Oxygen Therapy
- Hospital
---
