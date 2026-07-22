---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tesorio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tesorio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tesorio
provider_slug: tesorio
scheme_count: 1
schemes:
- applies_to: https://mcp.tesorio.com/v1/mcp
  browser_based: true
  flow: authorizationCode
  name: TesorioMCPOAuth
  scheme: oauth2.1
  sources:
  - https://help.tesorio.com/en/articles/14050733-mcp-server-connect-ai-tools-to-tesorio
  type: oauth2
slug: tesorio-authentication
source_filename: tesorio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.tesorio.com/en/articles/14050733-mcp-server-connect-ai-tools-to-tesorio\ndocs: https://help.tesorio.com/en/articles/14050733-mcp-server-connect-ai-tools-to-tesorio\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  notes: >-\n    Tesorio does not publish a general-purpose public REST API with its own auth\n    docs. The documented programmatic surface is the hosted MCP server at\n    https://mcp.tesorio.com/v1/mcp, which authenticates with OAuth 2.1 via a\n    secure browser-based login using existing Tesorio credentials. No static API\n    key is issued; the password is never stored locally by the client.\nschemes:\n  - name: TesorioMCPOAuth\n    type: oauth2\n    scheme: oauth2.1\n    flow: authorizationCode\n    browser_based: true\n    applies_to: https://mcp.tesorio.com/v1/mcp\n    sources: [https://help.tesorio.com/en/articles/14050733-mcp-server-connect-ai-tools-to-tesorio]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesorio/refs/heads/main/authentication/tesorio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Financial Operations
- Accounts Receivable
- Cash Flow
- Collections
- Treasury
- FinTech
- MCP
---
