---
api_key_in: []
auth_types:
- none
- bearer-visitor-token
description: ''
kind: authentication
layout: security
method: probed
name: Koloma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koloma secures its APIs with none and bearer-visitor-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Koloma
provider_slug: koloma
scheme_count: 2
schemes:
- applies_to:
  - mcp:initialize
  - mcp:tools/list
  - mcp:GetBusinessDetails
  - mcp:SearchInSite
  - mcp:SearchSiteApiDocs
  - mcp:BrowseWixRESTDocsMenu
  - mcp:ReadFullDocsArticle
  - mcp:ReadFullDocsMethodSchema
  evidence: Live POST tools/list and tools/call GetBusinessDetails both returned HTTP 200 with no Authorization header.
  name: anonymous
  sources:
  - mcp/koloma-mcp.yml
  type: none
- applies_to:
  - mcp:CallWixSiteAPI
  - mcp:ExecuteWixAPI
  bearerFormat: Wix visitor access token
  evidence: inputSchema for CallWixSiteAPI marks visitorToken required; GenerateVisitorToken is documented as the mint step. Confirmed from the live tools/list response.
  issued_by: mcp:GenerateVisitorToken
  name: visitorToken
  passed_as: tool argument (visitorToken), not an HTTP header
  scheme: bearer
  sources:
  - mcp/koloma-mcp-tools-list.json
  type: http
slug: koloma-authentication
source_filename: koloma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://www.kolomacalifornia.com/_api/mcp\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nsummary:\n  types: [none, bearer-visitor-token]\n  api_key_in: []\n  oauth2_flows: []\n  note: 'Koloma publishes no developer API and no API key, OAuth or OIDC surface. The\n    only authenticated surface found is the Wix-platform site MCP endpoint on the Koloma\n    California host, whose discovery and read-only tools answer anonymously and whose\n    write/API-call tools require a visitor access token minted by the server itself.'\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - mcp:initialize\n  - mcp:tools/list\n  - mcp:GetBusinessDetails\n  - mcp:SearchInSite\n  - mcp:SearchSiteApiDocs\n  - mcp:BrowseWixRESTDocsMenu\n  - mcp:ReadFullDocsArticle\n  - mcp:ReadFullDocsMethodSchema\n  evidence: 'Live POST tools/list and tools/call GetBusinessDetails both returned HTTP\n    200\
  \ with no Authorization header.'\n  sources: [mcp/koloma-mcp.yml]\n- name: visitorToken\n  type: http\n  scheme: bearer\n  bearerFormat: Wix visitor access token\n  issued_by: mcp:GenerateVisitorToken\n  passed_as: tool argument (visitorToken), not an HTTP header\n  applies_to:\n  - mcp:CallWixSiteAPI\n  - mcp:ExecuteWixAPI\n  evidence: 'inputSchema for CallWixSiteAPI marks visitorToken required; GenerateVisitorToken\n    is documented as the mint step. Confirmed from the live tools/list response.'\n  sources: [mcp/koloma-mcp-tools-list.json]\nnegative_findings:\n  openid_configuration: not published (404/400 on all hosts)\n  oauth_authorization_server: not published (404/400 on all hosts)\n  oauth_protected_resource: not published (404/400 on all hosts)\n  api_keys: no developer key issuance surface exists\n  openapi_security_schemes: no OpenAPI published\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://www.kolomacalifornia.com/_api/mcp\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koloma/refs/heads/main/authentication/koloma-authentication.yml
summary_line: none/bearer-visitor-token · 2 schemes
tags:
- Company
- Energy
- Clean Energy
- Hydrogen
- Natural Hydrogen
- Geologic Hydrogen
- Exploration
- Geoscience
- Climate Tech
- Decarbonization
---
