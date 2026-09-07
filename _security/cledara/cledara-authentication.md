---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cledara-api-openapi.json
  format: json
  label: Cledara API
  slug: cledara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cledara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cledara declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cledara
provider_slug: cledara
scheme_count: 2
schemes:
- api: Cledara API
  applied_to: all 3 operations (declared per-operation; the spec sets no top-level security)
  description: API key issued from the Cledara Web Application.
  format: 'Authorization: Bearer <your-api-key>'
  header: Authorization
  id: BearerAuth
  in: header
  observed_failures:
  - body: '{"message":"Missing or invalid Authorization header. Expected: Bearer <token>","error":{"method":"GET","url":"/v0/applications","status":401,"cledaraType":"cledaraError","errorId":29317748}}'
    probed: '2026-09-05'
    status: 401
    trigger: no Authorization header
  - probed: '2026-09-05'
    status: 401
    trigger: syntactically valid but unknown bearer token
  - source: openapi/cledara-api-openapi.json (declared, not probed)
    status: 403
    trigger: authenticated principal lacks privileges for the account
  permission_model: '"Each key grants the same level of access as the user who created it." There are no scopes, no per-key permission grants and no service accounts — the key inherits the creating user''s role, which makes key custody the whole authorization story. Cledara''s own docs say to treat it like a password.'
  provisioning:
    docs: https://www.cledara.com/blog/introducing-the-cledara-api
    location: Cledara web app → Settings → Profile Details → API Keys
    requires_sales_contact: false
    self_serve: true
  rotation:
    documented: false
    note: No published rotation, expiry or revocation policy for API keys was found.
  scheme: bearer
  source: openapi/cledara-api-openapi.json#/components/securitySchemes/BearerAuth
  type: http
- api: Cledara SaaS Market Data Hub MCP Server
  authorization_endpoint: https://data.cledara.com/authorize
  description: OAuth 2.1 authorization-code (PKCE S256) or client-credentials, per RFC 8414 metadata.
  grant_types:
  - authorization_code
  - client_credentials
  header: Authorization
  id: DataHubOAuth
  in: header
  issuer: https://data.cledara.com
  observed_failures:
  - body: '{"error":"Unauthorized"}'
    note: No WWW-Authenticate challenge is returned and no /.well-known/oauth-protected-resource is served, so RFC 9728 resource-metadata discovery does not work; a client must know to look for the same-origin authorization-server document.
    probed: '2026-09-05'
    status: 401
    trigger: POST /mcp tools/list with no token
  pkce:
    required_methods:
    - S256
  provisioning:
    mechanism: dynamic client registration (RFC 7591) at https://data.cledara.com/oauth/register
    note: DCR plus a public-client auth method means an MCP client can onboard itself with no human provisioning step — the strongest agent-onboarding signal on this provider.
    requires_sales_contact: false
    self_serve: true
  registration_endpoint: https://data.cledara.com/oauth/register
  revocation_endpoint: https://data.cledara.com/oauth/revoke
  scopes:
  - mcp:read
  source: https://data.cledara.com/.well-known/oauth-authorization-server
  token_endpoint: https://data.cledara.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: cledara-authentication
source_filename: cledara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://api-docs.cledara.com/ (info.description of openapi/cledara-api-openapi.json),\n  https://www.cledara.com/blog/introducing-the-cledara-api,\n  https://data.cledara.com/.well-known/oauth-authorization-server (probed 2026-09-05)\nprovider: Cledara\nproviderId: cledara\nsummary: >-\n  Two unrelated authentication models, one per surface. The workspace REST API uses a\n  static Bearer API key minted in the Cledara web app; the market-data MCP endpoint uses\n  OAuth 2.1 with dynamic client registration and PKCE. Neither surface issues the other's\n  credential.\nschemes:\n  - id: BearerAuth\n    api: Cledara API\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <your-api-key>'\n    description: API key issued from the Cledara Web Application.\n    source: openapi/cledara-api-openapi.json#/components/securitySchemes/BearerAuth\n    applied_to: all 3 operations\
  \ (declared per-operation; the spec sets no top-level security)\n    provisioning:\n      self_serve: true\n      location: Cledara web app → Settings → Profile Details → API Keys\n      docs: https://www.cledara.com/blog/introducing-the-cledara-api\n      requires_sales_contact: false\n    permission_model: >-\n      \"Each key grants the same level of access as the user who created it.\" There are no\n      scopes, no per-key permission grants and no service accounts — the key inherits the\n      creating user's role, which makes key custody the whole authorization story. Cledara's\n      own docs say to treat it like a password.\n    rotation:\n      documented: false\n      note: No published rotation, expiry or revocation policy for API keys was found.\n    observed_failures:\n      - status: 401\n        trigger: no Authorization header\n        body: '{\"message\":\"Missing or invalid Authorization header. Expected: Bearer <token>\",\"error\":{\"method\":\"GET\",\"url\":\"/v0/applications\"\
  ,\"status\":401,\"cledaraType\":\"cledaraError\",\"errorId\":29317748}}'\n        probed: '2026-09-05'\n      - status: 401\n        trigger: syntactically valid but unknown bearer token\n        probed: '2026-09-05'\n      - status: 403\n        trigger: authenticated principal lacks privileges for the account\n        source: openapi/cledara-api-openapi.json (declared, not probed)\n  - id: DataHubOAuth\n    api: Cledara SaaS Market Data Hub MCP Server\n    type: oauth2\n    in: header\n    header: Authorization\n    description: OAuth 2.1 authorization-code (PKCE S256) or client-credentials, per RFC 8414 metadata.\n    source: https://data.cledara.com/.well-known/oauth-authorization-server\n    issuer: https://data.cledara.com\n    authorization_endpoint: https://data.cledara.com/authorize\n    token_endpoint: https://data.cledara.com/oauth/token\n    registration_endpoint: https://data.cledara.com/oauth/register\n    revocation_endpoint: https://data.cledara.com/oauth/revoke\n    grant_types:\n\
  \      - authorization_code\n      - client_credentials\n    pkce:\n      required_methods:\n        - S256\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - none\n    scopes:\n      - mcp:read\n    provisioning:\n      self_serve: true\n      mechanism: dynamic client registration (RFC 7591) at https://data.cledara.com/oauth/register\n      requires_sales_contact: false\n      note: >-\n        DCR plus a public-client auth method means an MCP client can onboard itself with no\n        human provisioning step — the strongest agent-onboarding signal on this provider.\n    observed_failures:\n      - status: 401\n        trigger: 'POST /mcp tools/list with no token'\n        body: '{\"error\":\"Unauthorized\"}'\n        probed: '2026-09-05'\n        note: No WWW-Authenticate challenge is returned and no /.well-known/oauth-protected-resource is served, so RFC 9728 resource-metadata discovery does not work; a client must know to look for the same-origin authorization-server\
  \ document.\nnot_supported:\n  - mutualTLS\n  - openIdConnect\n  - apiKey (query or cookie)\n  - HMAC request signing\n  - basic auth\ngaps:\n  - The REST API has no OAuth, no scopes and no delegated-access story; every integration\n    runs as a human user's full permissions.\n  - No documented key rotation, expiry or revocation for the REST API key.\n  - The MCP endpoint returns a bare 401 with no WWW-Authenticate header and serves no\n    /.well-known/oauth-protected-resource, so a conforming MCP client cannot auto-discover\n    its authorization server from the challenge.\nmaintainers:\n  - FN: Kin Lane\n    email: kinlane@gmail.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/authentication/cledara-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- SaaS Management
- Software Spending
- Spend Management
- Subscription Management
- Virtual Cards
- Expense Management
- FinOps
- MCP
- Market Data
---
