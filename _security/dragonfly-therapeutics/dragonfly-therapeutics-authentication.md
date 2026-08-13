---
api_key_in: []
auth_types:
- none
- bearer-visitor-token
description: ''
kind: authentication
layout: security
method: probed
name: Dragonfly Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dragonfly Therapeutics secures its APIs with none and bearer-visitor-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dragonfly Therapeutics
provider_slug: dragonfly-therapeutics
scheme_count: 2
schemes:
- applies_to:
  - tools/list
  - GetBusinessDetails
  - SearchInSite
  - SearchSiteApiDocs
  - GenerateVisitorToken
  evidence: POST tools/list and POST tools/call GetBusinessDetails both returned HTTP 200 with no credential of any kind supplied.
  name: anonymous
  type: none
- applies_to:
  - CallWixSiteAPI
  - ExecuteWixAPI
  evidence: Both tools declare a required visitorToken property in the inputSchema returned by tools/list, and the llms.txt states GenerateVisitorToken must be called first.
  issuance: Obtained anonymously from the GenerateVisitorToken tool on the same endpoint; no account, registration or API key is required.
  name: visitorToken
  scheme: bearer
  type: http
slug: dragonfly-therapeutics-authentication
source_filename: dragonfly-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.dragonflytx.com/_api/mcp\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nnote: >-\n  Derived from live observation of the only callable surface this company serves — the\n  Wix-provisioned Site MCP endpoint. There is no OpenAPI, no securitySchemes block and no\n  first-party auth documentation to read, so derive-authentication.py produced nothing; this\n  profile records what the endpoint actually did when probed anonymously on 2026-08-12.\nsummary:\n  types: [none, bearer-visitor-token]\n  api_key_in: []\n  oauth2_flows: []\n  oauth_discovery: absent\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - tools/list\n  - GetBusinessDetails\n  - SearchInSite\n  - SearchSiteApiDocs\n  - GenerateVisitorToken\n  evidence: >-\n    POST tools/list and POST tools/call GetBusinessDetails both returned HTTP 200 with no\n    credential of any kind supplied.\n- name: visitorToken\n\
  \  type: http\n  scheme: bearer\n  applies_to:\n  - CallWixSiteAPI\n  - ExecuteWixAPI\n  issuance: >-\n    Obtained anonymously from the GenerateVisitorToken tool on the same endpoint; no account,\n    registration or API key is required.\n  evidence: >-\n    Both tools declare a required visitorToken property in the inputSchema returned by\n    tools/list, and the llms.txt states GenerateVisitorToken must be called first.\ndiscovery:\n- path: /.well-known/oauth-authorization-server\n  status: 400\n  present: false\n- path: /.well-known/oauth-protected-resource\n  status: 400\n  present: false\n- path: /.well-known/openid-configuration\n  status: 400\n  present: false\nscopes: []\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://www.dragonflytx.com/_api/mcp\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragonfly-therapeutics/refs/heads/main/authentication/dragonfly-therapeutics-authentication.yml
summary_line: none/bearer-visitor-token · 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Immunotherapy
- Oncology
- Life Sciences
- Clinical Stage
- Drug Discovery
- Healthcare
---
