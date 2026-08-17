---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Spot Runner Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot Runner declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Spot Runner
provider_slug: spot-runner
scheme_count: 0
schemes: []
slug: spot-runner-authentication
source_filename: spot-runner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: >-\n  mcp/spot-runner-mcp-tools.json (live tools/list, HTTP 200) + llms/spot-runner-llms.txt\n  (https://www.spotrunner.com/llms.txt, HTTP 200)\nscope: >-\n  This profile covers the ONLY public API surface Spot Runner exposes — the Wix Site MCP\n  endpoint. Spot Runner publishes no REST/GraphQL developer API, so there are no OpenAPI\n  securitySchemes to derive from.\nsurfaces:\n- name: Wix Site MCP endpoint\n  url: https://www.spotrunner.com/_api/mcp\n  transport: streamable-http (JSON-RPC 2.0)\n  connect_auth: none\n  connect_evidence: >-\n    An anonymous POST of {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"} returned HTTP 200 with\n    the full 9-tool manifest. No Authorization header, API key or OAuth challenge was required\n    to connect or to enumerate tools. A bare GET on the same URL returns 401.\n  schemes:\n  - id: anonymous-connect\n    type: none\n    applies_to:\n    - tools/list\n    - GetBusinessDetails\n\
  \    - SearchInSite\n    - SearchSiteApiDocs\n    - BrowseWixRESTDocsMenu\n    - ReadFullDocsArticle\n    - ReadFullDocsMethodSchema\n    description: >-\n      Discovery and read tools require no credential. They return only information already\n      public on the site.\n  - id: visitor-token\n    type: bearer-like\n    obtained_via: GenerateVisitorToken\n    passed_as: visitorToken argument on the tool call (not an HTTP header)\n    applies_to:\n    - CallWixSiteAPI\n    - ExecuteWixAPI\n    required: true\n    description: >-\n      Acting tools require a short-lived Wix visitor access token. The agent calls\n      GenerateVisitorToken to create a visitor session, then passes the returned token as the\n      visitorToken argument. The token carries visitor-level authority only — it can query\n      site data, start a booking or begin a purchase on an anonymous visitor's behalf, but it\n      does not authenticate a Spot Runner customer.\n    evidence: >-\n      inputSchema for CallWixSiteAPI\
  \ requires [visitorToken, url, method]; ExecuteWixAPI\n      requires [code, reason, hasMutations, sourceDocUrls, visitorToken].\n  oauth:\n    supported: false\n    evidence: >-\n      /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both\n      404/400 on every Spot Runner host (see well-known/spot-runner-well-known.yml).\n  openid_connect:\n    supported: false\n    evidence: /.well-known/openid-configuration returns no document on any host\n- name: Advertiser portal backend\n  url: https://api.spotrunner.com\n  public: false\n  documented: false\n  observed_flow: passwordless-email (magic link)\n  evidence: >-\n    The portal SPA bundle (https://advertiser.spotrunner.com/assets/index-B9BDGY7_.js, HTTP\n    200) names /v1/auth/email/login and /v1/auth/token against the api.spotrunner.com base.\n    This is the portal's own private backend; Spot Runner publishes no reference or spec for\n    it, so no scheme is claimed beyond the observed login shape.\n\
  notes: >-\n  No scopes/ artifact is emitted: there is no OAuth surface and no permission model to\n  enumerate. Nothing here was invented — every scheme is read off a live response or the\n  provider's own llms.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot-runner/refs/heads/main/authentication/spot-runner-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- AdTech
- Connected TV
- CTV
- Online Video
- Contextual Advertising
- Agentic AI
- Media Planning
---
