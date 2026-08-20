---
api_key_in: []
auth_types:
- none
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Aro Biotherapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aro Biotherapeutics secures its APIs with none and session-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aro Biotherapeutics
provider_slug: aro-biotherapeutics
scheme_count: 2
schemes:
- applies_to:
  - 'MCP method: initialize'
  - 'MCP method: tools/list'
  description: Discovery is unauthenticated. POST tools/list to https://www.arobiotx.com/_api/mcp with no credentials returns HTTP 200 and the full 9-tool manifest with input schemas.
  evidence:
    fetched: '2026-08-06'
    http_status: 200
    request: POST {"jsonrpc":"2.0","id":1,"method":"tools/list"}
    url: https://www.arobiotx.com/_api/mcp
  name: anonymous
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  description: Actions taken on a visitor's behalf require a visitor access token. An agent calls the GenerateVisitorToken tool, which takes no parameters and creates an anonymous visitor session, then passes the returned token as the visitorToken argument. This is a self-service anonymous session, not an identity credential — no registration, account or approval step exists.
  evidence:
    fetched: '2026-08-06'
    http_status: 200
    source: 'tools/list inputSchema: visitorToken listed in required[] for CallWixSiteAPI and ExecuteWixAPI'
    url: https://www.arobiotx.com/_api/mcp
  issued_by: GenerateVisitorToken
  name: visitorToken
  passed_as: visitorToken parameter on the tool call (not an HTTP header)
  type: session-token
slug: aro-biotherapeutics-authentication
source_filename: aro-biotherapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://www.arobiotx.com/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nscope: >-\n  Aro Biotherapeutics publishes no OpenAPI, no developer portal and no API key programme, so there\n  is no securityScheme to derive from. The only callable surface on the domain is the Wix-provided\n  Site MCP endpoint, and this profile records the auth model that endpoint actually enforces, as\n  observed live.\nsummary:\n  types:\n  - none\n  - session-token\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_discovery: true\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - 'MCP method: initialize'\n  - 'MCP method: tools/list'\n  description: >-\n    Discovery is unauthenticated. POST tools/list to https://www.arobiotx.com/_api/mcp with no\n    credentials returns HTTP 200 and the full 9-tool manifest with input schemas.\n  evidence:\n    url: https://www.arobiotx.com/_api/mcp\n\
  \    request: POST {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}\n    http_status: 200\n    fetched: '2026-08-06'\n- name: visitorToken\n  type: session-token\n  issued_by: GenerateVisitorToken\n  passed_as: visitorToken parameter on the tool call (not an HTTP header)\n  applies_to:\n  - CallWixSiteAPI\n  - ExecuteWixAPI\n  description: >-\n    Actions taken on a visitor's behalf require a visitor access token. An agent calls the\n    GenerateVisitorToken tool, which takes no parameters and creates an anonymous visitor session,\n    then passes the returned token as the visitorToken argument. This is a self-service anonymous\n    session, not an identity credential — no registration, account or approval step exists.\n  evidence:\n    url: https://www.arobiotx.com/_api/mcp\n    source: 'tools/list inputSchema: visitorToken listed in required[] for CallWixSiteAPI and ExecuteWixAPI'\n    http_status: 200\n    fetched: '2026-08-06'\nobservations:\n- >-\n  GET (rather than POST)\
  \ on https://www.arobiotx.com/_api/mcp returns HTTP 401 application/json,\n  confirming the endpoint enforces the MCP transport contract rather than answering everything 200.\n- >-\n  No OAuth metadata is published: /.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource both return 400 on this origin.\n- >-\n  ExecuteWixAPI is annotated destructiveHint:true and executes caller-supplied JavaScript against\n  the Wix REST API under the anonymous visitor session. Anyone on the internet can obtain that\n  session, so the effective trust boundary is whatever the Wix visitor role permits on this site.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aro-biotherapeutics/refs/heads/main/authentication/aro-biotherapeutics-authentication.yml
summary_line: none/session-token · 2 schemes
tags:
- Company
- Biotechnology
- Therapeutics
- Genetic Medicine
- Life Sciences
- Pharmaceuticals
- MCP
---
