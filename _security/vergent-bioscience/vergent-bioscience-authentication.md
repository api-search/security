---
api_key_in: []
auth_types: []
description: Vergent Bioscience publishes no REST/GraphQL API and therefore no OpenAPI securitySchemes. The only callable surface on its own hosts is the anonymous Wix Site MCP endpoint, whose access model was established by direct probe and is stated in the company's own llms.txt.
kind: authentication
layout: security
method: probed
name: Vergent Bioscience Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vergent Bioscience declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Vergent Bioscience
provider_slug: vergent-bioscience
scheme_count: 0
schemes: []
slug: vergent-bioscience-authentication
source_filename: vergent-bioscience-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://www.vergentbio.com/_api/mcp\ndescription: >-\n  Vergent Bioscience publishes no REST/GraphQL API and therefore no OpenAPI securitySchemes.\n  The only callable surface on its own hosts is the anonymous Wix Site MCP endpoint, whose\n  access model was established by direct probe and is stated in the company's own llms.txt.\nsurfaces:\n  - name: Site MCP endpoint\n    url: https://www.vergentbio.com/_api/mcp\n    schemes:\n      - type: none\n        applies_to: transport + tools/list + read tools (GetBusinessDetails, SearchInSite, docs tools)\n        evidence: >-\n          POST tools/list with no Authorization header returned HTTP 200 and the full 9-tool\n          manifest on 2026-09-02; a tools/call of GetBusinessDetails likewise returned 200.\n        docs: https://www.vergentbio.com/llms.txt\n        docs_quote: 'No authentication required to connect to the MCP endpoint'\n      - type: bearer-visitor-token\n    \
  \    applies_to: CallWixSiteAPI, ExecuteWixAPI\n        obtained_via: GenerateVisitorToken tool on the same endpoint\n        anonymous_issuance: true\n        evidence: >-\n          The probed inputSchema for both tools marks visitorToken as required; the\n          GenerateVisitorToken tool takes no parameters and mints a session for any caller.\n        note: >-\n          This is a session identity, not a credential the provider issues to a developer.\n          There is no key, no signup, and no account.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\nscopes: none\nnotes:\n  - >-\n    scopes/ is deliberately absent: there is no OAuth surface to enumerate, and an empty\n    scopes artifact would misrepresent the model.\n  - >-\n    Company hosts serve no /.well-known/openid-configuration or /.well-known/\n    oauth-authorization-server (both HTTP 400 — see well-known/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vergent-bioscience/refs/heads/main/authentication/vergent-bioscience-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Healthcare
- Medical Imaging
- Oncology
- Surgery
- Clinical Trials
- Model Context Protocol
---
