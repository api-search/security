---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Agrodesignstudio Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgroDesign Studios declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AgroDesign Studios
provider_slug: agrodesignstudio
scheme_count: 2
schemes:
- applies_to:
  - https://www.agrobox.jp/_api/mcp
  - https://www.agrodesign.shop/_api/mcp
  description: 'The MCP endpoints accept an unauthenticated JSON-RPC POST. initialize and tools/list both returned HTTP 200 with no WWW-Authenticate challenge and no invalid_token error. Both /llms.txt files state it explicitly: "connecting to the MCP endpoint requires no authentication" / "MCP エンドポイントへの接続に認証は不要です".'
  name: none
  type: none
  x-evidence:
    fetched: '2026-09-13'
    http_status: 200
    url: https://www.agrobox.jp/_api/mcp
- applies_to:
  - https://www.agrobox.jp/_api/mcp
  - https://www.agrodesign.shop/_api/mcp
  caller_supplied: false
  description: The GenerateVisitorToken tool takes no parameters and returns a site visitor access token that must be passed to CallWixSiteAPI and ExecuteWixAPI. This is a server-minted anonymous session identifier, not a credential the caller supplies or an account the caller holds — it carries public-visitor scope only.
  issued_by: Wix Site MCP server
  name: visitor-token
  type: session-token
slug: agrodesignstudio-authentication
source_filename: agrodesignstudio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://www.agrobox.jp/_api/mcp\ndocs: https://www.agrobox.jp/llms.txt\nsummary: >-\n  AgroDesign Studios publishes no first-party API and therefore no API credential of any kind —\n  no API key, no OAuth client registration, no developer account. The only machine-callable\n  surface is the Wix platform Site MCP endpoint on each of its two Wix-hosted sites, and that\n  surface is ANONYMOUS: no authentication is required to connect, and the only token involved is\n  a visitor-scoped session token the server itself mints on request.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - https://www.agrobox.jp/_api/mcp\n  - https://www.agrodesign.shop/_api/mcp\n  description: >-\n    The MCP endpoints accept an unauthenticated JSON-RPC POST. initialize and tools/list both\n    returned HTTP 200 with no WWW-Authenticate challenge and no invalid_token error. Both\n    /llms.txt files state it explicitly: \"connecting to the MCP\
  \ endpoint requires no\n    authentication\" / \"MCP エンドポイントへの接続に認証は不要です\".\n  x-evidence:\n    fetched: '2026-09-13'\n    url: https://www.agrobox.jp/_api/mcp\n    http_status: 200\n- name: visitor-token\n  type: session-token\n  applies_to:\n  - https://www.agrobox.jp/_api/mcp\n  - https://www.agrodesign.shop/_api/mcp\n  description: >-\n    The GenerateVisitorToken tool takes no parameters and returns a site visitor access token\n    that must be passed to CallWixSiteAPI and ExecuteWixAPI. This is a server-minted anonymous\n    session identifier, not a credential the caller supplies or an account the caller holds — it\n    carries public-visitor scope only.\n  issued_by: Wix Site MCP server\n  caller_supplied: false\noauth:\n  supported: false\n  discovery_probed: true\n  note: >-\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource were probed\n    on all three company hosts. The Wix edge answers HTTP 400 for every /.well-known/* path on\n    the\
  \ two Wix hosts, and the corporate site answers HTTP 404. No OAuth metadata is published.\nscope_model:\n  present: false\n  note: >-\n    No OAuth scope surface exists, so no scopes/ artifact is emitted. Authorization is binary and\n    implicit — the server exposes only what an anonymous visitor can already reach on the public\n    website.\nexposure:\n  note: >-\n    Because the endpoint is anonymous, the practical access-control boundary is whatever the Wix\n    visitor-token scope permits. Both /llms.txt files assert that only publicly accessible site\n    information is available through it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrodesignstudio/refs/heads/main/authentication/agrodesignstudio-authentication.yml
summary_line: 2 schemes
tags:
- Agriculture
- AgTech
- Biotechnology
- Life Sciences
- Structural Biology
- Drug Discovery
- Crop Protection
- Contract Research
- Laboratory Automation
- Japan
- MCP
- Company
---
