---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Peer39 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peer39 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Peer39
provider_slug: peer39
scheme_count: 2
schemes:
- description: 'Session-token bearer auth. Every call under /api/external/ carries `Authorization: Bearer <sessionId>`, where the sessionId is minted by the login endpoint below. This is NOT OAuth 2.0 and NOT a long-lived API key — it is a short-lived server-issued session id obtained from username + password.'
  expiry:
    client_behavior: The reference client caches the sessionId and refreshes it 60s before expiry; on a 401 mid-flight it invalidates the cache, re-logs-in once, and retries the original request exactly once.
    source: expirationInSeconds field on the login response
  format: Bearer <sessionId>
  header: Authorization
  id: peer39-session
  in: header
  scheme: bearer
  token_endpoint:
    method: POST
    path: /api/external/login
    probe:
      fetched: '2026-08-12'
      http_status: 401
      note: POSTed with empty credentials; the endpoint exists and rejects with 401 rather than 404, consistent with the documented "401 Peer39 login failed" behavior.
      url: https://app.peer39.com/api/external/login
    request_body:
      password: string
      username: string
    response_shape:
      expirationInSeconds: integer
      result.sessionId: string
    url: https://app.peer39.com/api/external/login
  type: http
- description: A per-account "system name" string that must accompany category-creation calls (POST /api/external/customcategories). It is an account-scoped identifier, not a secret credential, and is surfaced to customers on their account page in app.peer39.com. Omitting or mis-setting it returns Peer39 error code 63 ("Invalid system parameter").
  header: system
  id: peer39-system-header
  in: header
  required_for:
  - POST /api/external/customcategories
  type: apiKey
slug: peer39-authentication
source_filename: peer39-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: >-\n  https://github.com/awhite07/p39-custom-category-mcp/blob/main/src/auth/client.ts\n  and src/api/client.ts — the first-party-authored Peer39 MCP server (\"UNLICENSED —\n  internal Peer39 project\", package name \"@peer39/mcp-server\"), corroborated by a live\n  unauthenticated probe of https://app.peer39.com/api/external/login (HTTP 401).\napi: Peer39 External API\nbase_url: https://app.peer39.com\n\nnote: >-\n  Peer39 publishes no public API reference page. This profile is derived from the\n  publicly readable source of Peer39's own MCP server client plus live probes of the\n  API host. Every value below is read from that client or observed on the wire — none\n  is inferred. Peer39 distributes its API documentation as PDFs handed out by account\n  managers (the MCP source cites \"Peer39 PDF\" as the source of its language-code and\n  wildcard rules), so there is no machine-readable securityScheme document to derive from.\n\
  \nschemes:\n  - id: peer39-session\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <sessionId>'\n    description: >-\n      Session-token bearer auth. Every call under /api/external/ carries\n      `Authorization: Bearer <sessionId>`, where the sessionId is minted by the login\n      endpoint below. This is NOT OAuth 2.0 and NOT a long-lived API key — it is a\n      short-lived server-issued session id obtained from username + password.\n    token_endpoint:\n      method: POST\n      path: /api/external/login\n      url: https://app.peer39.com/api/external/login\n      request_body:\n        username: string\n        password: string\n      response_shape:\n        result.sessionId: string\n        expirationInSeconds: integer\n      probe:\n        fetched: '2026-08-12'\n        url: https://app.peer39.com/api/external/login\n        http_status: 401\n        note: >-\n          POSTed with empty credentials; the endpoint exists and\
  \ rejects with 401 rather\n          than 404, consistent with the documented \"401 Peer39 login failed\" behavior.\n    expiry:\n      source: expirationInSeconds field on the login response\n      client_behavior: >-\n        The reference client caches the sessionId and refreshes it 60s before expiry;\n        on a 401 mid-flight it invalidates the cache, re-logs-in once, and retries the\n        original request exactly once.\n\n  - id: peer39-system-header\n    type: apiKey\n    in: header\n    header: system\n    description: >-\n      A per-account \"system name\" string that must accompany category-creation calls\n      (POST /api/external/customcategories). It is an account-scoped identifier, not a\n      secret credential, and is surfaced to customers on their account page in\n      app.peer39.com. Omitting or mis-setting it returns Peer39 error code 63\n      (\"Invalid system parameter\").\n    required_for:\n      - POST /api/external/customcategories\n\nauthorization:\n \
  \ model: role-based, provisioned by Peer39 — not self-service\n  required_roles:\n    - name: External API\n      note: >-\n        The login account must carry this role or login returns 401. The MCP server's\n        troubleshooting table instructs the user to \"ask your Peer39 integration manager\n        to add it\", confirming roles are granted by Peer39 staff rather than self-served.\n    - name: RTB Buyer\n  scoping:\n    - field: buyerId\n      note: numeric buyer account id; calls are scoped to buyer accounts the credential owns\n    - field: partnerId\n      note: >-\n        numeric DSP partner id (e.g. 841 = Microsoft Advertising / Xandr,\n        1407 = The Trade Desk); a category belongs to a buyer + partner pair\n  errors_on_scope_mismatch:\n    - code: 6\n      message: Account ID not found\n    - code: 31\n      message: Invalid Account ID\n    - code: 51\n      message: Invalid Buyer ID\n\nsignup:\n  self_service: false\n  how: >-\n    Credentials are issued through a\
  \ Peer39 account/integration manager. There is no\n    developer portal, no API key self-service page, and no public signup that yields\n    API credentials. https://www.peer39.com/signup/ is a marketing signup, not a\n    developer credential flow.\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key: false\n\nrelated_oauth_note: >-\n  An OAuth 2.1 authorization server DOES exist in the Peer39 MCP orbit — the remote\n  \"Peer39 MCP Connector\" beta at https://mcp-connector.scatter-brain.ai serves RFC 8414\n  and RFC 9728 metadata and supports PKCE S256 + RFC 7591 dynamic client registration.\n  It is NOT hosted on a Peer39-controlled domain and it does not authenticate the Peer39\n  API itself — it stores the user's Peer39 username/password encrypted and exchanges them\n  for a session id behind the scenes. It is recorded in mcp/peer39-mcp.yml, not here.\n\ncross_reference:\n  errors: errors/peer39-problem-types.yml\n  conventions: conventions/peer39-conventions.yml\n \
  \ mcp: mcp/peer39-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peer39/refs/heads/main/authentication/peer39-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Contextual Advertising
- AdTech
- Brand Safety
- Programmatic Advertising
- Contextual Targeting
- CTV
- MarTech
- Advertising
- Custom Categories
- DSP
---
