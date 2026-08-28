---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Photys Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Photys Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Photys Therapeutics
provider_slug: photys-therapeutics
scheme_count: 0
schemes: []
slug: photys-therapeutics-authentication
source_filename: photys-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.photys.com/_api/mcp\nnote: >-\n  Derived from live probes of the only machine-readable surface Photys serves (the Wix Site\n  MCP endpoint) plus the company's own published llms.txt. There is no OpenAPI document, so\n  there are no securitySchemes to read; nothing below is inferred from a spec.\nsurfaces:\n- name: Photys Site MCP\n  url: https://www.photys.com/_api/mcp\n  schemes:\n  - type: none\n    applies_to:\n    - initialize\n    - tools/list\n    - GetBusinessDetails\n    - SearchInSite\n    - SearchSiteApiDocs\n    - GenerateVisitorToken\n    - ReadFullDocsArticle\n    - ReadFullDocsMethodSchema\n    - BrowseWixRESTDocsMenu\n    evidence: >-\n      Anonymous POST with no Authorization header returned HTTP 200 for initialize and\n      tools/list on 2026-08-26.\n  - type: bearer\n    name: visitorToken\n    issued_by: GenerateVisitorToken (MCP tool, anonymous — no credential required to mint one)\n    applies_to:\n\
  \    - CallWixSiteAPI\n    - ExecuteWixAPI\n    evidence: >-\n      Both tools declare visitorToken in their required inputSchema properties; the published\n      llms.txt states \"Must be called before making any CallWixSiteAPI request if no visitor\n      token is already available in context\" and \"No authentication required to connect to\n      the MCP endpoint\".\noauth: false\napi_keys: false\nmutual_tls: false\nopenid_connect: false\nsummary: >-\n  Fully anonymous. No account, key, or OAuth flow exists — the session token that gates the\n  two write-capable tools is minted on demand by an unauthenticated tool call, and the server\n  exposes only public site content.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photys-therapeutics/refs/heads/main/authentication/photys-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Clinical Trials
- Oncology
- Protein Degradation
- MCP
---
