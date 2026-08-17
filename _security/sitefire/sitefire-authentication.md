---
api_key_in: []
api_specs:
- filename: sitefire-book-demo-api-openapi.yml
  format: yaml
  label: Sitefire Book Demo API
  slug: sitefire-book-demo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/openapi/sitefire-book-demo-api-openapi.yml
auth_types:
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Sitefire Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sitefire secures its APIs with oauth2 and none across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sitefire
provider_slug: sitefire
scheme_count: 2
schemes:
- applies_to: https://app.sitefire.ai/api/mcp
  authorization_server:
    dynamic_client_registration: true
    file: sitefire-mcp-authorization-server.json
    id_token_signing_alg_values_supported:
    - RS256
    - HS256
    - ES256
    issuer: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1
    jwks_uri: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/jwks.json
    metadata_spec: RFC 8414 (OAuth 2.0 Authorization Server Metadata)
    metadata_url: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/oauth-authorization-server
    operator: Supabase (third-party identity platform used by Sitefire)
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
    - none
    userinfo_endpoint: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/userinfo
  bearer_methods_supported:
  - header
  discovery:
    canonical_well_known_note: The metadata document is real and machine-readable but is served from /api/mcp/oauth-metadata rather than the RFC 9728 canonical location /.well-known/oauth-protected-resource. The canonical path returns the app's single-page-app HTML shell (soft 200), not a document. Because of that, no WellKnown pointer is emitted for this provider.
    canonical_well_known_path_served: false
    challenge_header: 'WWW-Authenticate: Bearer resource_metadata="https://app.sitefire.ai/api/mcp/oauth-metadata"'
    file: sitefire-mcp-protected-resource.json
    protected_resource_metadata: https://app.sitefire.ai/api/mcp/oauth-metadata
    protected_resource_metadata_spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)
  flows:
  - authorizationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    refreshSupported: true
    registrationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/clients/register
    scopes:
    - openid
    - profile
    - email
    - phone
    - offline_access
    tokenUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token
  name: mcp-oauth
  sources:
  - https://app.sitefire.ai/api/mcp/oauth-metadata
  type: oauth2
  user_experience: Browser sign-in to a Sitefire account. Documented per client - Claude.ai custom connector, `claude mcp add --transport http --scope user sitefire https://app.sitefire.ai/api/mcp`, ChatGPT developer-mode connector, and `codex mcp add sitefire --url https://app.sitefire.ai/api/mcp` followed by `codex mcp login sitefire`.
- applies_to: https://sitefire.ai/api
  description: The Book Demo API is documented as public and unauthenticated. The OpenAPI declares no securitySchemes and no security requirement on either operation.
  name: none
  note: See lifecycle/sitefire-lifecycle.yml - both documented Book Demo routes were probed on 2026-08-13 and neither resolved, so the unauthenticated posture could not be exercised end to end.
  sources:
  - https://sitefire.ai/llms.txt
  - openapi/sitefire-book-demo-api-openapi.yml
  type: none
slug: sitefire-authentication
source_filename: sitefire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://app.sitefire.ai/api/mcp/oauth-metadata\ndocs: https://sitefire.ai/docs/mcp.md\nnotes: >-\n  Sitefire runs two authentication postures, and they are opposites. The hosted\n  MCP server (Spark) is protected by OAuth 2.1 and advertises real RFC 9728\n  protected-resource metadata: an unauthenticated POST to the MCP endpoint\n  returns 401 with a WWW-Authenticate Bearer challenge naming the metadata URL,\n  which resolves to a Supabase-hosted authorization server publishing RFC 8414\n  metadata (PKCE S256, dynamic client registration, authorization_code +\n  refresh_token). The public Book Demo REST API declares no security scheme at\n  all and its own llms.txt states \"No API key required. The API is public.\"\n  Nothing was derived from OpenAPI securitySchemes because the only published\n  spec declares none - derive-authentication.py returned zero schemes for this\n  provider. Everything below was probed live.\nsummary:\n\
  \  types: [oauth2, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  surfaces: 2\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://app.sitefire.ai/api/mcp\n  sources: [https://app.sitefire.ai/api/mcp/oauth-metadata]\n  bearer_methods_supported: [header]\n  discovery:\n    protected_resource_metadata: https://app.sitefire.ai/api/mcp/oauth-metadata\n    protected_resource_metadata_spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n    challenge_header: 'WWW-Authenticate: Bearer resource_metadata=\"https://app.sitefire.ai/api/mcp/oauth-metadata\"'\n    canonical_well_known_path_served: false\n    canonical_well_known_note: >-\n      The metadata document is real and machine-readable but is served from\n      /api/mcp/oauth-metadata rather than the RFC 9728 canonical location\n      /.well-known/oauth-protected-resource. The canonical path returns the\n      app's single-page-app HTML shell (soft 200), not a document. Because of\n      that, no WellKnown\
  \ pointer is emitted for this provider.\n    file: sitefire-mcp-protected-resource.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/token\n    registrationUrl: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/clients/register\n    refreshSupported: true\n    pkce: [S256, plain]\n    scopes: [openid, profile, email, phone, offline_access]\n  authorization_server:\n    issuer: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1\n    operator: Supabase (third-party identity platform used by Sitefire)\n    metadata_spec: RFC 8414 (OAuth 2.0 Authorization Server Metadata)\n    metadata_url: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/oauth-authorization-server\n    jwks_uri: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/jwks.json\n    userinfo_endpoint: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/oauth/userinfo\n\
  \    dynamic_client_registration: true\n    id_token_signing_alg_values_supported: [RS256, HS256, ES256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n    file: sitefire-mcp-authorization-server.json\n  user_experience: >-\n    Browser sign-in to a Sitefire account. Documented per client - Claude.ai\n    custom connector, `claude mcp add --transport http --scope user sitefire\n    https://app.sitefire.ai/api/mcp`, ChatGPT developer-mode connector, and\n    `codex mcp add sitefire --url https://app.sitefire.ai/api/mcp` followed by\n    `codex mcp login sitefire`.\n- name: none\n  type: none\n  applies_to: https://sitefire.ai/api\n  sources: [https://sitefire.ai/llms.txt, openapi/sitefire-book-demo-api-openapi.yml]\n  description: >-\n    The Book Demo API is documented as public and unauthenticated. The OpenAPI\n    declares no securitySchemes and no security requirement on either operation.\n  note: >-\n    See lifecycle/sitefire-lifecycle.yml\
  \ - both documented Book Demo routes were\n    probed on 2026-08-13 and neither resolved, so the unauthenticated posture\n    could not be exercised end to end.\nx-evidence:\n- url: https://app.sitefire.ai/api/mcp\n  method: POST\n  http_status: 401\n  note: JSON-RPC tools/list; returned {\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32000,\"message\":\"Unauthorized\"}} plus the WWW-Authenticate Bearer challenge\n  checked: '2026-08-13'\n- url: https://app.sitefire.ai/api/mcp/oauth-metadata\n  http_status: 200\n  content_type: application/json\n  checked: '2026-08-13'\n- url: https://qhfesxmsojjleewjufcn.supabase.co/auth/v1/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  checked: '2026-08-13'\n- url: https://app.sitefire.ai/.well-known/oauth-protected-resource\n  http_status: 200\n  content_type: text/html\n  note: SPA shell, not a document - rejected as a soft 200\n  checked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitefire/refs/heads/main/authentication/sitefire-authentication.yml
summary_line: oauth2/none · 2 schemes
tags:
- Company
- Generative Engine Optimization
- AI Visibility
- Marketing
- SEO
- Analytics
- Artificial Intelligence
- Content Generation
- MCP
- Agent
---
