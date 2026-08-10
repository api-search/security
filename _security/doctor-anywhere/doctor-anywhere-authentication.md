---
api_key_in: []
auth_types:
- none
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Doctor Anywhere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doctor Anywhere secures its APIs with none and session-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Doctor Anywhere
provider_slug: doctor-anywhere
scheme_count: 2
schemes:
- applies_to:
  - https://doctoranywhere.co.th/_api/mcp
  - https://www.doctoranywhere.my/_api/mcp
  - https://doctoranywhere.co.id/_api/mcp
  description: Connecting to the site MCP endpoint and calling tools/list requires no credentials. The published llms.txt states "No authentication required to connect to the MCP endpoint" and "Only public information accessible on the site is available".
  evidence: POST tools/list returned HTTP 200 with 9 tools and no Authorization header, 2026-08-04.
  name: anonymous-mcp
  type: none
- applies_to:
  - https://doctoranywhere.co.th/_api/mcp
  - https://www.doctoranywhere.my/_api/mcp
  - https://doctoranywhere.co.id/_api/mcp
  consuming_tools:
  - CallWixSiteAPI
  - ExecuteWixAPI
  description: Acting on a visitor's behalf requires a visitor access token minted by the GenerateVisitorToken tool and then passed as the required visitorToken argument to CallWixSiteAPI and ExecuteWixAPI. The token is scoped to a visitor session over public site data; there is no user login, API key or OAuth scope surface.
  evidence: mcp/doctor-anywhere-mcp-tools-list.json
  name: wix-visitor-token
  token_issuer_tool: GenerateVisitorToken
  type: session-token
slug: doctor-anywhere-authentication
source_filename: doctor-anywhere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://doctoranywhere.co.th/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nnote: 'Doctor Anywhere publishes no OpenAPI, so no securitySchemes could be derived. The\n  only publicly documented authentication contract on any Doctor Anywhere host is the\n  Wix Site MCP visitor-session model advertised in the regional llms.txt files and\n  confirmed by an anonymous tools/list.'\nsummary:\n  types: [none, session-token]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: anonymous-mcp\n  type: none\n  applies_to:\n  - https://doctoranywhere.co.th/_api/mcp\n  - https://www.doctoranywhere.my/_api/mcp\n  - https://doctoranywhere.co.id/_api/mcp\n  description: 'Connecting to the site MCP endpoint and calling tools/list requires no\n    credentials. The published llms.txt states \"No authentication required to connect to\n    the MCP endpoint\" and \"Only public information\
  \ accessible on the site is available\".'\n  evidence: 'POST tools/list returned HTTP 200 with 9 tools and no Authorization header,\n    2026-08-04.'\n- name: wix-visitor-token\n  type: session-token\n  applies_to:\n  - https://doctoranywhere.co.th/_api/mcp\n  - https://www.doctoranywhere.my/_api/mcp\n  - https://doctoranywhere.co.id/_api/mcp\n  description: 'Acting on a visitor''s behalf requires a visitor access token minted by\n    the GenerateVisitorToken tool and then passed as the required visitorToken argument\n    to CallWixSiteAPI and ExecuteWixAPI. The token is scoped to a visitor session over\n    public site data; there is no user login, API key or OAuth scope surface.'\n  token_issuer_tool: GenerateVisitorToken\n  consuming_tools: [CallWixSiteAPI, ExecuteWixAPI]\n  evidence: mcp/doctor-anywhere-mcp-tools-list.json\nnot_published:\n  api_keys: 'No public API key issuance — there is no Doctor Anywhere developer portal or\n    signup for API credentials.'\n  oauth2: 'No /.well-known/oauth-authorization-server\
  \ or /.well-known/openid-configuration\n    on any host (see well-known/doctor-anywhere-well-known.yml).'\n  platform_api: 'api.doctoranywhere.com is an Apigee gateway serving Doctor Anywhere''s own\n    apps; anonymous requests return an Apigee ApplicationNotFound fault and no auth\n    challenge or documentation is exposed.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctor-anywhere/refs/heads/main/authentication/doctor-anywhere-authentication.yml
summary_line: none/session-token · 2 schemes
tags:
- Company
- Healthcare
- Telehealth
- Telemedicine
- Digital Health
- Health Screening
- Corporate Wellness
- Singapore
- Southeast Asia
- Model Context Protocol
---
