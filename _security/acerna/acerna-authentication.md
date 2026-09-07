---
anonymous_access: true
api_key_in: []
auth_types:
- none
- session-token
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Acerna Authentication
name_suffix: Authentication
oauth_flows: []
overview: aceRNA Technologies secures its APIs with none and session-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: aceRNA Technologies
provider_slug: acerna
scheme_count: 2
schemes:
- applies_to:
  - 'MCP method: tools/list'
  - 'MCP method: tools/call (GetBusinessDetails, SearchInSite, SearchSiteApiDocs, GenerateVisitorToken)'
  description: Discovery is unauthenticated. POST tools/list to https://www.acernatec.com/_api/mcp with no credentials returns HTTP 200 and the full 9-tool manifest with JSON Schema inputs. A tools/call of GetBusinessDetails with no credentials also returned 200.
  evidence:
    fetched: '2026-09-06'
    http_status: 200
    request: POST {"jsonrpc":"2.0","id":1,"method":"tools/list"}
    url: https://www.acernatec.com/_api/mcp
  name: anonymous
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  description: Actions taken on a visitor's behalf require a visitor access token. An agent calls the GenerateVisitorToken tool, which takes no parameters and creates an anonymous visitor session, then passes the returned token as the visitorToken argument. This is a self-service anonymous session, not an identity credential — there is no registration, account, key issuance or approval step anywhere on this domain.
  evidence:
    fetched: '2026-09-06'
    http_status: 200
    source: 'tools/list inputSchema: visitorToken listed in required[] for CallWixSiteAPI and ExecuteWixAPI'
    url: https://www.acernatec.com/_api/mcp
  issued_by: GenerateVisitorToken
  name: visitorToken
  passed_as: visitorToken parameter on the tool call (not an HTTP header)
  type: session-token
slug: acerna-authentication
source_filename: acerna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.acernatec.com/_api/mcp\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nscope: >-\n  aceRNA Technologies publishes no OpenAPI, no developer portal and no API key programme, so there\n  is no securityScheme to derive from. The only callable surface on the domain is the Wix-provided\n  Site MCP endpoint, and this profile records the auth model that endpoint actually enforces, as\n  observed live on 2026-09-06.\nsummary:\n  types:\n  - none\n  - session-token\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_discovery: true\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - 'MCP method: tools/list'\n  - 'MCP method: tools/call (GetBusinessDetails, SearchInSite, SearchSiteApiDocs, GenerateVisitorToken)'\n  description: >-\n    Discovery is unauthenticated. POST tools/list to https://www.acernatec.com/_api/mcp with no\n    credentials returns HTTP 200 and the\
  \ full 9-tool manifest with JSON Schema inputs. A\n    tools/call of GetBusinessDetails with no credentials also returned 200.\n  evidence:\n    url: https://www.acernatec.com/_api/mcp\n    request: POST {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}\n    http_status: 200\n    fetched: '2026-09-06'\n- name: visitorToken\n  type: session-token\n  issued_by: GenerateVisitorToken\n  passed_as: visitorToken parameter on the tool call (not an HTTP header)\n  applies_to:\n  - CallWixSiteAPI\n  - ExecuteWixAPI\n  description: >-\n    Actions taken on a visitor's behalf require a visitor access token. An agent calls the\n    GenerateVisitorToken tool, which takes no parameters and creates an anonymous visitor session,\n    then passes the returned token as the visitorToken argument. This is a self-service anonymous\n    session, not an identity credential — there is no registration, account, key issuance or\n    approval step anywhere on this domain.\n  evidence:\n    url: https://www.acernatec.com/_api/mcp\n\
  \    source: 'tools/list inputSchema: visitorToken listed in required[] for CallWixSiteAPI and ExecuteWixAPI'\n    http_status: 200\n    fetched: '2026-09-06'\nobservations:\n- >-\n  GET (rather than POST) on https://www.acernatec.com/_api/mcp returns HTTP 401 application/json\n  with {\"error\":\"invalid_token\",\"error_description\":\"Missing Authorization header\"}, confirming the\n  endpoint enforces the MCP transport contract rather than answering everything 200.\n- >-\n  No OAuth metadata is published: /.well-known/oauth-authorization-server,\n  /.well-known/oauth-protected-resource and /.well-known/oauth-protected-resource/_api/mcp all\n  return HTTP 400 on this origin, as does a control path under /.well-known/, so 400 is the Wix\n  catch-all for that prefix rather than a server fault.\n- >-\n  ExecuteWixAPI is annotated destructiveHint:true and executes caller-supplied JavaScript against\n  the Wix REST API under the anonymous visitor session. Anyone on the internet can obtain\
  \ that\n  session, so the effective trust boundary is whatever the Wix visitor role permits on this site —\n  which, on a marketing-only site with no store, bookings or members area installed, is narrow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acerna/refs/heads/main/authentication/acerna-authentication.yml
summary_line: none/session-token · 2 schemes
tags:
- Company
- Biotechnology
- Therapeutics
- Genetic Medicine
- Life Sciences
- Pharmaceuticals
- Japan
- MCP
---
