---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Aetherai Authentication
name_suffix: Authentication
oauth_flows: []
overview: aetherAI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: aetherAI
provider_slug: aetherai
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
  evidence: https://www.aetherai.com/_api/mcp
  id: anonymous
  note: 'Probed 2026-09-12 with no Authorization header: HTTP 200, 9 tools returned. The published llms.txt states plainly "No authentication required to connect to the MCP endpoint".'
  type: none
  verified: probed
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  evidence: https://www.aetherai.com/llms.txt
  id: visitor-token
  issuance: In-band. The client calls the GenerateVisitorToken tool, which creates a visitor session and returns an access token. No registration, no API key, no client credentials.
  note: The token is passed as a tool ARGUMENT, not as an HTTP Authorization header — a Wix design choice, not an aetherAI one. Scope is limited to what an anonymous site visitor may do.
  parameter: visitorToken
  type: bearer-in-parameter
  verified: probed
slug: aetherai-authentication
source_filename: aetherai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://www.aetherai.com/_api/mcp (live probe), https://www.aetherai.com/llms.txt\nsummary: >-\n  There is exactly one publicly callable aetherAI surface and it is ANONYMOUS. The Wix Site MCP\n  endpoint at https://www.aetherai.com/_api/mcp accepts initialize and tools/list with no\n  credential of any kind; a short-lived anonymous visitor token (minted in-band by the\n  GenerateVisitorToken tool) is required only before the two write-capable tools. aetherAI's\n  clinical products are behind a customer login at https://demo.aetherai.com/dpai/login/ and\n  publish no authentication documentation, no key-issuance flow, and no OAuth metadata.\n\nscope_of_this_profile: >-\n  This describes the website's agent endpoint, NOT aetherSlide / aetherWeb / Hema / Endo / Ortho.\n  Those have no public authentication surface to profile.\n\nschemes:\n  - id: anonymous\n    type: none\n    applies_to:\n      - initialize\n      - tools/list\n\
  \      - GetBusinessDetails\n      - SearchInSite\n      - SearchSiteApiDocs\n      - BrowseWixRESTDocsMenu\n      - ReadFullDocsArticle\n      - ReadFullDocsMethodSchema\n    verified: probed\n    evidence: https://www.aetherai.com/_api/mcp\n    note: >-\n      Probed 2026-09-12 with no Authorization header: HTTP 200, 9 tools returned. The published\n      llms.txt states plainly \"No authentication required to connect to the MCP endpoint\".\n  - id: visitor-token\n    type: bearer-in-parameter\n    applies_to:\n      - CallWixSiteAPI\n      - ExecuteWixAPI\n    parameter: visitorToken\n    issuance: >-\n      In-band. The client calls the GenerateVisitorToken tool, which creates a visitor session and\n      returns an access token. No registration, no API key, no client credentials.\n    verified: probed\n    evidence: https://www.aetherai.com/llms.txt\n    note: >-\n      The token is passed as a tool ARGUMENT, not as an HTTP Authorization header — a Wix design\n      choice, not an\
  \ aetherAI one. Scope is limited to what an anonymous site visitor may do.\n\noauth:\n  supported: false\n  discovery_probed:\n    - url: https://www.aetherai.com/.well-known/oauth-authorization-server\n      status: 400\n    - url: https://www.aetherai.com/.well-known/oauth-protected-resource/_api/mcp\n      status: 400\n    - url: https://www.aetherai.com/.well-known/openid-configuration\n      status: 400\n  note: >-\n    No OAuth 2.0 or OpenID Connect metadata is served on any host. No scopes/ artifact is written,\n    because there is no scope surface to derive one from.\n\napi_keys:\n  supported: false\n  note: aetherAI issues no public API keys and documents no key lifecycle.\n\ngated_surfaces:\n  - name: aetherAI DPAI (demo / customer application)\n    url: https://demo.aetherai.com/dpai/login/\n    status: 200\n    note: >-\n      A login-gated single-page application. Every path under it, including /api/ and every spec\n      path probed, returns either the SPA shell or a 404\
  \ to an unauthenticated client. No\n      credentials were used and none were sought.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetherai/refs/heads/main/authentication/aetherai-authentication.yml
summary_line: 2 schemes
tags:
- Healthcare
- Digital Pathology
- Medical Imaging
- Artificial Intelligence
- Diagnostics
- Machine Learning
- Medical Devices
- Life Sciences
- MCP
- Taiwan
---
