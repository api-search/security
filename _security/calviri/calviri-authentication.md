---
api_key_in: []
auth_types: []
description: 'Calviri publishes no product API and therefore no API-key, OAuth or OIDC program. The only callable surface on its host is the Wix-provisioned site MCP endpoint, and that endpoint is ANONYMOUS: an unauthenticated POST of `initialize` and of `tools/list` both returned 200 on 2026-08-09 with no credential of any kind. Write-side calls are gated only by a visitor access token that the server itself mints anonymously via the GenerateVisitorToken tool — there is no authorization server, no client registration and no scope surface. Derived from the live probe, not from a spec: there is no OpenAPI to read securitySchemes from.'
kind: authentication
layout: security
method: probed
name: Calviri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calviri declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Calviri
provider_slug: calviri
scheme_count: 0
schemes: []
slug: calviri-authentication
source_filename: calviri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://www.calviri.com/_api/mcp\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\ndescription: >-\n  Calviri publishes no product API and therefore no API-key, OAuth or OIDC\n  program. The only callable surface on its host is the Wix-provisioned site MCP\n  endpoint, and that endpoint is ANONYMOUS: an unauthenticated POST of\n  `initialize` and of `tools/list` both returned 200 on 2026-08-09 with no\n  credential of any kind. Write-side calls are gated only by a visitor access\n  token that the server itself mints anonymously via the GenerateVisitorToken\n  tool — there is no authorization server, no client registration and no scope\n  surface. Derived from the live probe, not from a spec: there is no OpenAPI to\n  read securitySchemes from.\napis:\n- name: Calviri Site MCP\n  url: https://www.calviri.com/_api/mcp\n  schemes:\n  - id: anonymous\n    type: none\n    in: n/a\n    description:\
  \ >-\n      No credential is required to connect, initialize, or list tools. The\n      server exposes only information already public on www.calviri.com.\n    evidence:\n      url: https://www.calviri.com/_api/mcp\n      method: 'POST tools/list (no Authorization header)'\n      http_status: 200\n      fetched: '2026-08-09'\n  - id: visitor-token\n    type: bearer-like\n    in: request body\n    parameter: visitorToken\n    description: >-\n      CallWixSiteAPI and ExecuteWixAPI require a `visitorToken` argument. The\n      token is obtained by calling the GenerateVisitorToken tool on the same\n      anonymous session; it identifies a visitor session, not a registered\n      developer, and no signup or key issuance is involved.\n    minted_by: GenerateVisitorToken\noauth:\n  present: false\n  authorization_server: null\n  protected_resource_metadata: null\n  notes: >-\n    /.well-known/oauth-authorization-server returns 400 (Wix edge behaviour for\n    all /.well-known/* paths) and\n\
  \    /_api/mcp/.well-known/oauth-protected-resource returns 404. RFC 8414 and\n    RFC 9728 metadata are absent.\napi_keys:\n  present: false\nmutual_tls:\n  present: false\nx-evidence:\n- fetched: '2026-08-09'\n  url: https://www.calviri.com/_api/mcp\n  http_status: 200\n- fetched: '2026-08-09'\n  url: https://www.calviri.com/.well-known/oauth-authorization-server\n  http_status: 400\n- fetched: '2026-08-09'\n  url: https://www.calviri.com/_api/mcp/.well-known/oauth-protected-resource\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calviri/refs/heads/main/authentication/calviri-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Health
- Cancer Diagnostics
- Vaccines
- Veterinary
- Animal Health
- Research
---
