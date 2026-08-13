---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Leadpages Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Leadpages secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Leadpages
provider_slug: leadpages
scheme_count: 2
schemes:
- availability: Pro plan and above (per the docs; the machine-readable pricing at /pricing.md marks "API access" as Yes on Pro, Business, Grow, Optimize and Scale, and No on Starter)
  description: API key issued from account dashboard settings, sent as a bearer token on every request. Documented as "best for server-to-server integrations", scoped to the account.
  format: Bearer lp_<api_key>
  in: header
  key_prefix: lp_
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://leadpages.com/developers/docs
  type: http
- availability: all plans, including the free trial
  description: OAuth 2.0 authorization-code flow with PKCE, used for the MCP server and user-facing integrations. Documented as "no credentials shared with third parties"; tokens refresh automatically.
  flows:
  - authorizationUrl: https://leadpages.com/api/mcp/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://leadpages.com/api/mcp/oauth/register
    scope_count: 11
    scopes_ref: scopes/leadpages-scopes.yml
    tokenUrl: https://leadpages.com/api/mcp/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
  name: oauth2
  sources:
  - https://leadpages.com/developers/docs
  - https://leadpages.com/.well-known/oauth-authorization-server
  type: oauth2
slug: leadpages-authentication
source_filename: leadpages-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://leadpages.com/developers/docs\ndocs: https://leadpages.com/developers/docs\nnote: >-\n  Derived from the provider's own developer documentation and its RFC 8414 /\n  RFC 9728 discovery documents, not from an OpenAPI — Leadpages publishes no\n  OpenAPI of its own. The spec served at https://leadpages.com/openapi.json\n  belongs to HTML Pub, a sibling brand, and was deliberately not used as a source\n  here (see conventions/leadpages-conventions.yml).\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  dynamic_client_registration: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: \"Bearer lp_<api_key>\"\n  key_prefix: lp_\n  description: >-\n    API key issued from account dashboard settings, sent as a bearer token on every\n    request. Documented as \"best for server-to-server\
  \ integrations\", scoped to the\n    account.\n  availability: Pro plan and above (per the docs; the machine-readable pricing at\n    /pricing.md marks \"API access\" as Yes on Pro, Business, Grow, Optimize and Scale,\n    and No on Starter)\n  sources: [https://leadpages.com/developers/docs]\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow with PKCE, used for the MCP server and\n    user-facing integrations. Documented as \"no credentials shared with third\n    parties\"; tokens refresh automatically.\n  availability: all plans, including the free trial\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://leadpages.com/api/mcp/oauth/authorize\n    tokenUrl: https://leadpages.com/api/mcp/oauth/token\n    registrationUrl: https://leadpages.com/api/mcp/oauth/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_post]\n    scope_count: 11\n\
  \    scopes_ref: scopes/leadpages-scopes.yml\n  sources:\n  - https://leadpages.com/developers/docs\n  - https://leadpages.com/.well-known/oauth-authorization-server\ndocs_endpoints:\n  documented_in_docs_page:\n  - POST /oauth/authorize\n  - POST /oauth/token\n  discovered_in_metadata:\n  - https://leadpages.com/api/mcp/oauth/authorize\n  - https://leadpages.com/api/mcp/oauth/token\n  - https://leadpages.com/api/mcp/oauth/register\n  discrepancy_note: >-\n    The docs page shows bare \"/oauth/authorize\" and \"/oauth/token\" paths while the\n    RFC 8414 metadata publishes them under /api/mcp/oauth/. Both are recorded; the\n    metadata document is the machine-readable authority.\nobserved:\n- {url: 'https://mcp.leadpages.com/mcp', unauthenticated_status: 401, body: '{\"error\":\"Unauthorized\"}'}\n- {url: 'https://leadpages.com/api/a2a', unauthenticated_status: 401, body: '{\"error\":\"Unauthorized\"}'}\n- note: >-\n    Both agent surfaces reject anonymous calls with a bare JSON {\"\
  error\":\"Unauthorized\"}\n    and no WWW-Authenticate challenge pointing at the protected-resource metadata,\n    so RFC 9728 discovery is published but not advertised on the 401 itself.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://leadpages.com/developers/docs', status: 200}\n  - {url: 'https://leadpages.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://mcp.leadpages.com/mcp', status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadpages/refs/heads/main/authentication/leadpages-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Landing Pages
- Marketing
- Conversion Optimization
- A/B Testing
- Website Builder
- Lead Generation
- Content Management
- Agents
- Analytics
---
