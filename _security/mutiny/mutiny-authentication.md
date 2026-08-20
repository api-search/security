---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mutiny Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mutiny declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Mutiny
provider_slug: mutiny
scheme_count: 0
schemes: []
slug: mutiny-authentication
source_filename: mutiny-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.mutinyhq.com/.well-known/oauth-authorization-server\ndocs: https://help.mutinyhq.com/articles/5003451538-connecting-mutiny-to-claude\nsummary: >-\n  Mutiny's only machine-callable surface is its hosted MCP server, and it is protected by a full OAuth\n  2.1 authorization-code flow with mandatory PKCE and RFC 7591 dynamic client registration. There is no\n  API-key path, no personal access token, and no public REST API to authenticate against.\napis:\n- api: Mutiny MCP Server\n  base_url: https://mcp.mutinyhq.com/mcp\n  security_schemes:\n  - id: mutiny_mcp_oauth\n    type: oauth2\n    profile: OAuth 2.1 as required by the MCP authorization specification\n    issuer: https://mcp.mutinyhq.com\n    flows:\n    - type: authorization_code\n      authorization_endpoint: https://mcp.mutinyhq.com/oauth/authorize\n      token_endpoint: https://mcp.mutinyhq.com/oauth/token\n      pkce_required: true\n      code_challenge_methods_supported:\n\
  \      - S256\n      response_types_supported:\n      - code\n      token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - none\n      scopes:\n      - read_asset_groups\n      - create_asset_groups\n      - publish_asset_groups\n      - read_library_content\n      - manage_library_content\n    dynamic_client_registration:\n      supported: true\n      spec: RFC 7591\n      endpoint: https://mcp.mutinyhq.com/oauth/register\n      note: >-\n        Anonymous client registration is what lets Claude web/Desktop/Code register themselves as\n        connectors without a human copying a client_id out of a developer portal.\n    discovery:\n      authorization_server_metadata: https://mcp.mutinyhq.com/.well-known/oauth-authorization-server\n      protected_resource_metadata: https://mcp.mutinyhq.com/.well-known/oauth-protected-resource\n      specs:\n      - RFC 8414\n      - RFC 9728\n      - RFC 7636 (PKCE)\n      - RFC 7591 (DCR)\n    refresh:\n      supported: false\n\
  \      note: >-\n        grant_types_supported declares authorization_code only; no refresh_token grant is advertised in\n        the metadata, so a client must re-run the authorization flow when the access token expires.\n  unauthenticated_behaviour:\n    endpoint: https://mcp.mutinyhq.com/mcp\n    method: POST\n    http_status: 401\n    body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Authentication failed.\"},\"id\":null}'\n    checked: '2026-08-13'\n    gap: >-\n      The 401 carries no WWW-Authenticate header pointing at the protected-resource metadata. RFC 9728\n      and the MCP authorization spec expect that challenge so a client can discover the authorization\n      server automatically from a failed call; here a client must already know to fetch\n      /.well-known/oauth-protected-resource.\n- api: Mutiny application (app.mutinyhq.com)\n  base_url: https://app.mutinyhq.com\n  security_schemes:\n  - id: session\n    type: session\n    note: >-\n      Interactive\
  \ browser session only. Every path probed on app.mutinyhq.com — including\n      /.well-known/* and /openapi.json — returns 401. Enterprise plans add SSO per the pricing page.\n      No developer-facing credential is issued.\napi_keys:\n  supported: false\n  note: Mutiny publishes no API key, secret key, or personal access token surface.\nnotes: >-\n  Everything above is read from live, anonymous probes of Mutiny's own discovery documents on\n  2026-08-13, plus the connection instructions in Mutiny's help centre. No securityScheme was derived\n  from an OpenAPI document because Mutiny publishes none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutiny/refs/heads/main/authentication/mutiny-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Enterprise
- Sales
- Marketing
- Go-To-Market
- Artificial Intelligence
- AI Agents
- Sales Enablement
- Account Based Marketing
- Workflow-Automation
- MCP
---
