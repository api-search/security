---
api_key_in:
- header
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pubmatic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PubMatic secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PubMatic
provider_slug: pubmatic
scheme_count: 3
schemes:
- credential_source: https://help.pubmatic.com/activate/reference/get-started-with-pubmatic-apis
  description: PubMatic-issued Bearer token ("PubToken") generated through the PubMatic API or UI. Used by the Claude Desktop MCP extension and by direct MCP clients.
  in: header
  name: PubToken
  observed:
    fetched: '2026-08-13'
    http_status: 401
    url: https://mcp.pubmatic.com/mcp
    www_authenticate: Bearer error="invalid_token", error_description="The access token is invalid or expired"
  parameter: Authorization
  scheme: bearer
  sources:
  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/Claude_Desktop_Extension/MCP_Claude_Setup_Readme_External.md
  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/DSP%20Onboarding/DSP_onboarding_integration_guide.md
  type: http
- description: API key authentication for all requests to the MCP Server. Obtained from a PubMatic representative; there is no self-service issuance.
  in: header
  name: X-API-Key
  parameter: X-API-Key
  sources:
  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/Deal%20Management/README.md
  type: apiKey
- discovery:
    note: RFC 8414 / RFC 9728 discovery documents are NOT served on mcp.pubmatic.com, so an MCP client cannot resolve the authorization server programmatically from the 401 challenge.
    oauth_authorization_server: 404
    oauth_protected_resource: 404
  flows:
  - description: ChatGPT connectors select "OAuth" as the authentication type; the user is redirected to a PubMatic login page chosen by resource-type — /login/publisher for PUBLISHER (1), /login/activate for ACTIVATE ADVERTISER (14) — and returns an installed connector.
    flow: authorizationCode
    login_endpoint_pattern: https://mcp.pubmatic.com/login/{publisher|activate}
    scopes: []
    scopes_note: 'No scope vocabulary is published. Authorization is coarse: the user account must have "API access enabled", and the connector is bound to one resource. No scopes/ artifact is emitted because there is nothing real to record.'
  name: PubMatic OAuth (ChatGPT connector)
  sources:
  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/ChatGPT_Extension/MCP_ChatGPT_Setup_Readme_External.md
  type: oauth2
slug: pubmatic-authentication
source_filename: pubmatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/PubMatic/pubmatic-mcp-server\ndocs: https://help.pubmatic.com/activate/reference/get-started-with-pubmatic-apis\ndocs_status: gated\nnote: >-\n  DERIVED FROM NO OPENAPI — PubMatic publishes no OpenAPI/Swagger document anywhere this\n  pipeline could reach, so there are no securitySchemes to aggregate. Everything below is\n  transcribed from PubMatic's own published MCP integration guides and client setup\n  documents in github.com/PubMatic/pubmatic-mcp-server, plus one directly observed response\n  header. The canonical auth reference (help.pubmatic.com/activate/reference/\n  get-started-with-pubmatic-apis) is real but 302s into the ReadMe -> Auth0 -> Okta ->\n  apps.pubmatic.com customer login chain, so its contents could not be read.\nsummary:\n  types: [http, apiKey, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  multi_tenant: true\n  tenant_selector:\
  \ resource-id + resource-type\nschemes:\n- name: PubToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    PubMatic-issued Bearer token (\"PubToken\") generated through the PubMatic API or UI. Used\n    by the Claude Desktop MCP extension and by direct MCP clients.\n  credential_source: https://help.pubmatic.com/activate/reference/get-started-with-pubmatic-apis\n  sources:\n  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/Claude_Desktop_Extension/MCP_Claude_Setup_Readme_External.md\n  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/DSP%20Onboarding/DSP_onboarding_integration_guide.md\n  observed:\n    url: https://mcp.pubmatic.com/mcp\n    http_status: 401\n    www_authenticate: Bearer error=\"invalid_token\", error_description=\"The access token is invalid or expired\"\n    fetched: '2026-08-13'\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    API key authentication\
  \ for all requests to the MCP Server. Obtained from a PubMatic\n    representative; there is no self-service issuance.\n  sources:\n  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/Deal%20Management/README.md\n- name: PubMatic OAuth (ChatGPT connector)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    login_endpoint_pattern: https://mcp.pubmatic.com/login/{publisher|activate}\n    description: >-\n      ChatGPT connectors select \"OAuth\" as the authentication type; the user is redirected to\n      a PubMatic login page chosen by resource-type — /login/publisher for PUBLISHER (1),\n      /login/activate for ACTIVATE ADVERTISER (14) — and returns an installed connector.\n    scopes: []\n    scopes_note: >-\n      No scope vocabulary is published. Authorization is coarse: the user account must have\n      \"API access enabled\", and the connector is bound to one resource. No scopes/ artifact\n      is emitted because there is nothing real to record.\n  discovery:\n\
  \    oauth_authorization_server: 404\n    oauth_protected_resource: 404\n    note: >-\n      RFC 8414 / RFC 9728 discovery documents are NOT served on mcp.pubmatic.com, so an MCP\n      client cannot resolve the authorization server programmatically from the 401 challenge.\n  sources:\n  - https://github.com/PubMatic/pubmatic-mcp-server/blob/main/ChatGPT_Extension/MCP_ChatGPT_Setup_Readme_External.md\ntenancy:\n  description: >-\n    Every authenticated call is scoped to exactly one PubMatic resource. The pair is supplied\n    as query parameters on the MCP URL for ChatGPT (which cannot send custom headers) and as\n    extension configuration fields for Claude Desktop.\n  parameters:\n  - name: resource-id\n    required: true\n    issued_by: PubMatic Solutions Engineer\n  - name: resource-type\n    required: true\n    values: [PUBLISHER, DSP, BUYER, ACTIVATE ADVERTISER]\n    numeric_ids: {PUBLISHER: 1, ACTIVATE ADVERTISER: 14}\n  constraint: >-\n    resource-id and resource-type are fixed\
  \ at connector-creation time and cannot be changed;\n    a second account requires a second connector. Sessions must be fully logged out before\n    creating a connector for a different resource type or authentication misroutes.\n  example_url: https://mcp.pubmatic.com/mcp?resource-id=<resource-id>&resource-type=PUBLISHER\nlegacy_api_surface:\n  host: https://api.pubmatic.com\n  observed_status: 404 at root, 500 on unknown paths\n  gateway: Apigee\n  note: >-\n    api.pubmatic.com is live and fronts a SOAP-era publisher web service — unknown paths\n    return a soap:Fault naming\n    http://v1_0.webservices.publisher.core.pubmatic.com/ with errorCode ClassificationFailure\n    and errorMessage \"This is an invalid api.\" No OpenAPI, Swagger UI, /docs, /redoc or\n    GraphQL endpoint is exposed. Its authentication model is not publicly documented.\nx-evidence:\n- {url: 'https://mcp.pubmatic.com/mcp', http_status: 401, fetched: '2026-08-13'}\n- {url: 'https://help.pubmatic.com/activate/reference/get-started-with-pubmatic-apis',\
  \ http_status: 302, fetched: '2026-08-13'}\n- {url: 'https://api.pubmatic.com/', http_status: 404, fetched: '2026-08-13'}\n- {url: 'https://api.pubmatic.com/openapi.json', http_status: 500, fetched: '2026-08-13'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubmatic/refs/heads/main/authentication/pubmatic-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Advertising
- AdTech
- Programmatic Advertising
- Supply Side Platform
- SSP
- Header Bidding
- OpenWrap
- Prebid
- OpenRTB
- Connected TV
- CTV
- Mobile Advertising
- Commerce Media
- Retail Media
- Identity
- Curation
- Auction Packages
- Agentic AI
---
