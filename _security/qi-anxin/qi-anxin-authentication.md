---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Qi Anxin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qi Anxin declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Qi Anxin
provider_slug: qi-anxin
scheme_count: 1
schemes:
- applies_to:
  - https://webapi.ti.qianxin.com
  - https://ti.qianxin.com/api/v2/compromise
  - https://mcp.ti.qianxin.com/ti-stream-mcp
  - https://mcp.ti.qianxin.com/ti-mcp/sse
  description: Static per-account API key issued by the QAX Threat Intelligence Center console.
  example_request: 'curl ''https://webapi.ti.qianxin.com/ip/v3/reputation?param=<indicator>'' -H ''Api-Key: <your-key>'''
  id: ApiKeyHeader
  in: header
  name: Api-Key
  type: apiKey
slug: qi-anxin-authentication
source_filename: qi-anxin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://ti.qianxin.com/help/?path=ip-illustration30 (QAX Threat Intelligence\n  Center API help) and https://github.com/RedDrip7/qax-ti-mcp §五 安全认证说明; corroborated\n  by an unauthenticated live probe of https://webapi.ti.qianxin.com/\ndocs: https://ti.qianxin.com/help\nsummary: 'Every QAX Threat Intelligence surface — the REST API and the hosted MCP\n  server — authenticates with a single static API key carried in an `Api-Key` request\n  header. There is no OAuth, no OIDC, no bearer/JWT and no mTLS on the public surface.'\nschemes:\n- id: ApiKeyHeader\n  type: apiKey\n  in: header\n  name: Api-Key\n  applies_to:\n  - https://webapi.ti.qianxin.com\n  - https://ti.qianxin.com/api/v2/compromise\n  - https://mcp.ti.qianxin.com/ti-stream-mcp\n  - https://mcp.ti.qianxin.com/ti-mcp/sse\n  description: Static per-account API key issued by the QAX Threat Intelligence Center\n    console.\n  example_request: \"curl 'https://webapi.ti.qianxin.com/ip/v3/reputation?param=<indicator>'\\\
  \n    \\ -H 'Api-Key: <your-key>'\"\nkey_issuance:\n  self_service: false\n  route: 'Register an account at https://user.ti.qianxin.com/login, then request API\n    access from the platform administrators at ti_support@qianxin.com.'\n  console: https://ti.qianxin.com/\n  note: The provider does not publish a self-service key-generation flow on a page\n    reachable without an account; MCP keys are explicitly issued by contacting ti_support@qianxin.com.\nkey_management:\n  rotation_documented: false\n  ip_allowlist: 'Optional — IP allow-list binding is offered on separate application\n    (documented for the MCP service).'\n  scopes: false\n  scope_note: The API key is unscoped. No OAuth scope surface exists, so no scopes/\n    artifact is emitted.\ntransport:\n  tls: required\n  observed_tls_version: TLSv1.2\nunauthenticated_behaviour:\n  probed: '2026-08-26'\n  url: https://webapi.ti.qianxin.com/\n  http_status: 401\n  content_type: application/json; charset=utf-8\n  body: '{\"message\"\
  :\"No API key found in request\"}'\n  note: A missing key returns a JSON 401 rather than an HTML error page — the API\n    host is genuinely an API host, not the JS-rendered SPA that fronts ti.qianxin.com.\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qi-anxin/refs/heads/main/authentication/qi-anxin-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Threat Intelligence
- Endpoint Security
- Network Security
- Vulnerability Management
- MCP
- China
---
