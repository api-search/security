---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mobile Action Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobile Action secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mobile Action
provider_slug: mobile-action
scheme_count: 2
schemes:
- applies_to: https://api.mobileaction.co
  description: Account API key supplied as the `token` query parameter on every request. Balance is returned on GET /api-key and on the X-Credit-Remaining response header.
  in: query
  name: apiKeyToken
  parameter: token
  sources:
  - https://docs.mobileaction.co/guide/introduction
  type: apiKey
- applies_to: https://mcp.mobileaction.co/mcp
  description: 'The same account API key appended to the MCP server URL (https://mcp.mobileaction.co/mcp?token=YOUR-API-TOKEN). MobileAction documents this as credential-equivalent: "Anyone with this link can query your MobileAction data, so treat it like a password."'
  in: query
  name: mcpUrlToken
  parameter: token
  sources:
  - https://docs.mobileaction.co/mcp/server-setup
  type: apiKey
slug: mobile-action-authentication
source_filename: mobile-action-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.mobileaction.co/guide/introduction + https://docs.mobileaction.co/mcp/server-setup\ndocs: https://docs.mobileaction.co/guide/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  notes: 'One credential type covers the whole product: an account API key (\"token\") passed as a query\n    parameter. It authenticates the REST API and, appended to the MCP endpoint URL, the remote MCP server\n    too. Keys are metered against a credit balance. No OAuth, no OIDC, no bearer token, no mTLS is offered\n    on the API. Keys are issued by MobileAction (the MCP docs say \"the token provided by your Customer\n    Success Manager\") rather than self-served from a developer console, and access requires an active\n    API Solutions plan.'\nschemes:\n- name: apiKeyToken\n  type: apiKey\n  in: query\n  parameter: token\n  applies_to: https://api.mobileaction.co\n  description: Account API key\
  \ supplied as the `token` query parameter on every request. Balance is returned\n    on GET /api-key and on the X-Credit-Remaining response header.\n  sources:\n  - https://docs.mobileaction.co/guide/introduction\n- name: mcpUrlToken\n  type: apiKey\n  in: query\n  parameter: token\n  applies_to: https://mcp.mobileaction.co/mcp\n  description: 'The same account API key appended to the MCP server URL (https://mcp.mobileaction.co/mcp?token=YOUR-API-TOKEN).\n    MobileAction documents this as credential-equivalent: \"Anyone with this link can query your MobileAction\n    data, so treat it like a password.\"'\n  sources:\n  - https://docs.mobileaction.co/mcp/server-setup\nobserved_behaviour:\n- probe: GET https://api.mobileaction.co/api-key\n  result: HTTP 401, empty body\n- probe: GET https://api.mobileaction.co/api-key?token=INVALID\n  result: HTTP 401, empty body\n- probe: POST https://mcp.mobileaction.co/mcp tools/list (no token)\n  result: HTTP 200 - the tool catalogue with full input\
  \ schemas is readable ANONYMOUSLY; only invocation\n    needs the key.\nnot_offered:\n  oauth2: true\n  openIdConnect: true\n  mutualTLS: true\n  http_bearer: true\n  note: /.well-known/oauth-authorization-server and /.well-known/openid-configuration return 404 on both\n    api.mobileaction.co and mcp.mobileaction.co.\nunrelated_oauth_surface:\n  host: https://www.mobileaction.co\n  note: The WordPress marketing site does serve an OAuth 2.0 / OIDC discovery document with mcp:read /\n    mcp:write / mcp:woocommerce scopes. It belongs to a WordPress plugin on that site and does NOT authenticate\n    the intelligence API. Captured separately in scopes/mobile-action-scopes.yml and well-known/mobile-action-well-known.yml\n    so it is never mistaken for the API auth model.\nkey_handling:\n  rotation: from the MobileAction dashboard / via Customer Success\n  transport: query string\n  risk_note: Carrying the credential in the query string means it is exposed in browser history, proxy\n    logs\
  \ and server access logs, and in the MCP case it is pasted into a third-party AI client's connector\n    configuration. A header-based credential would be materially safer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobile-action/refs/heads/main/authentication/mobile-action-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- App Store Optimization
- ASO
- Mobile Marketing
- Apple Search Ads
- App Intelligence
- Ad Intelligence
- Market Intelligence
- Analytics
- MCP
- Agent Tools
- App Store Intelligence
- Mobile Measurement
---
