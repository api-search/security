---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Code Biotherapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Code Biotherapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Code Biotherapeutics
provider_slug: code-biotherapeutics
scheme_count: 0
schemes: []
slug: code-biotherapeutics-authentication
source_filename: code-biotherapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://www.codebiotx.com/_api/mcp\ndocs: https://www.codebiotx.com/llms.txt\nsummary: >-\n  Code Biotherapeutics publishes no developer program, no API keys and no OAuth. The only\n  callable surface on its host is the Wix site MCP server, which is anonymous by design:\n  discovery and read tools take no credential, and the two acting tools take a visitor\n  token that any caller can mint anonymously.\nsurfaces:\n- name: Code Bio Site MCP Server\n  url: https://www.codebiotx.com/_api/mcp\n  schemes:\n  - id: anonymous\n    type: none\n    applies_to:\n    - initialize\n    - tools/list\n    - GetBusinessDetails\n    - SearchInSite\n    - SearchSiteApiDocs\n    - BrowseWixRESTDocsMenu\n    - ReadFullDocsArticle\n    - ReadFullDocsMethodSchema\n    - GenerateVisitorToken\n    evidence: >-\n      POST tools/list with no Authorization header returned HTTP 200 and the full nine-tool\n      manifest on 2026-08-09.\n  - id: visitor-token\n\
  \    type: bearer-like\n    in: request-body\n    parameter: visitorToken\n    issued_by: GenerateVisitorToken\n    credential_required_to_obtain: none\n    applies_to:\n    - CallWixSiteAPI\n    - ExecuteWixAPI\n    evidence: >-\n      Both tools declare visitorToken in inputSchema.required; the tool descriptions and\n      llms.txt both instruct callers to obtain it from GenerateVisitorToken, which itself\n      takes no parameters and no credential.\noauth:\n  published: false\n  probes:\n  - url: https://www.codebiotx.com/.well-known/oauth-authorization-server\n    http_status: 400\n  - url: https://www.codebiotx.com/.well-known/oauth-protected-resource\n    http_status: 400\n  - url: https://www.codebiotx.com/_api/mcp/.well-known/oauth-protected-resource\n    http_status: 404\nopenid_connect:\n  published: false\n  probes:\n  - url: https://www.codebiotx.com/.well-known/openid-configuration\n    http_status: 400\napi_keys:\n  published: false\n  note: No developer portal, signup,\
  \ or key-issuance surface exists on codebiotx.com.\ncontrol:\n  url: https://www.codebiotx.com/zzz-nonexistent-control-path-98765\n  http_status: 404\n  note: >-\n    Control probe confirms the host does not soft-200 unknown paths, so the 400/404 misses\n    above are genuine absences rather than a catch-all.\nx-evidence:\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-biotherapeutics/refs/heads/main/authentication/code-biotherapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Genetic Medicine
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Rare Disease
- Drug Discovery
---
