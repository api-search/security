---
api_key_in: []
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wyndham Hotels Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wyndham Hotels & Resorts secures its APIs with none and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wyndham Hotels & Resorts
provider_slug: wyndham-hotels
scheme_count: 4
schemes:
- applies_to:
  - https://www.wyndhambusiness.com/wp-json/wp/v2
  - https://development.wyndhamhotels.com/wp-json/wp/v2
  evidence: 'GET /wp-json/ returns HTTP 200 with "authentication":

    {"application-passwords":{...}} only. Anonymous HTTP 200 confirmed on

    /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags,

    /wp/v2/users, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses,

    /wp/v2/comments, /wp/v2/search and /wp/v2/blocks on www.wyndhambusiness.com.

    '
  name: anonymous
  type: none
- applies_to:
  - https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server
  authorization_server_metadata: https://www.wyndhambusiness.com/.well-known/oauth-authorization-server
  bearer_methods_supported:
  - header
  client_credentials: false
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  evidence: 'Anonymous JSON-RPC tools/list returns 401 mcp_unauthorized with

    WWW-Authenticate: Bearer realm="https://www.wyndhambusiness.com",

    resource_metadata="https://www.wyndhambusiness.com/.well-known/oauth-protected-resource"

    '
  flows:
  - authorizationUrl: https://www.wyndhambusiness.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://www.wyndhambusiness.com/oauth/token
    scopes:
      mcp: Access the WordPress MCP server on www.wyndhambusiness.com
    tokenUrl: https://www.wyndhambusiness.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://www.wyndhambusiness.com
  name: wyndham-business-mcp-oauth
  note: 'PKCE S256 is the only code-challenge method and the token endpoint accepts no

    client authentication, which is the OAuth 2.1 public-client profile the MCP

    authorization spec expects. There is no registration endpoint; clients are

    expected to present a client-id metadata document URL.

    '
  protected_resource_metadata: https://www.wyndhambusiness.com/.well-known/oauth-protected-resource
  registration_endpoint: null
  resource: https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server
  response_types_supported:
  - code
  revocation_endpoint: https://www.wyndhambusiness.com/oauth/revoke
  source: well-known/wyndham-hotels-wyndhambusiness-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- application_passwords_endpoint: https://www.wyndhambusiness.com/wp-admin/authorize-application.php
  applies_to:
  - https://www.wyndhambusiness.com/wp-json/
  - https://development.wyndhamhotels.com/wp-json/
  evidence: 'GET /wp-json/wp/v2/settings returns 401 rest_forbidden;

    GET /wp-json/wp-abilities/v1/abilities returns 401 rest_forbidden;

    POST /wp-json/mcp/mcp-adapter-default-server returns 401 rest_forbidden.

    CORS advertises Authorization and X-WP-Nonce in access-control-allow-headers.

    '
  name: wordpress-privileged
  public: false
  type: cookie+nonce / application-password
- applies_to:
  - https://www.wyndhambusiness.com/ (Wyndham Business account)
  - https://www.wyndhamhotels.com/wyndham-rewards (Wyndham Rewards member)
  - https://wyndham.supplierone.co/ (supplier procurement, third party)
  name: human-login-walls
  note: 'Human sign-in surfaces only. Wyndham Business / Wyndham Direct access is

    approval-gated on a submitted request with a corporate code, company name,

    website URL and anticipated travel spend; none of it produces an API credential.

    '
  type: none-machine-readable
slug: wyndham-hotels-authentication
source_filename: wyndham-hotels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: |\n  live probes 2026-07-28 plus\n  https://www.wyndhambusiness.com/.well-known/oauth-authorization-server (RFC 8414)\n  and https://www.wyndhambusiness.com/.well-known/oauth-protected-resource (RFC 9728)\nnote: |\n  Probed rather than derived — Wyndham Hotels & Resorts publishes no OpenAPI or\n  other specification, so there are no securitySchemes to aggregate. Three distinct\n  authentication realms exist on the estate:\n\n    1. Anonymous. The WordPress REST APIs on www.wyndhambusiness.com and\n       development.wyndhamhotels.com answer read requests with no credential at all.\n       The /wp-json/ discovery document on wyndhambusiness.com advertises only\n       application-passwords, which is a WordPress admin flow, not a partner\n       credential path.\n    2. OAuth 2.1. The MCP server route on www.wyndhambusiness.com is a genuine\n       OAuth-protected resource with published RFC 8414 and RFC 9728 metadata,\n    \
  \   mandatory PKCE S256, public-client support via client_id_metadata_document,\n       and a single scope, `mcp`. It is standards-correct and completely\n       undocumented.\n    3. WordPress privileged. Settings, the wp-abilities registry and the second MCP\n       adapter reject anonymous callers with 401 and require a cookie + X-WP-Nonce\n       or an application password that Wyndham issues to no third party.\n\n  There is no API key program, no client-credentials grant, no self-serve\n  registration and no published route to request a credential of any kind.\nsummary:\n  types:\n  - none\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  public_read_requires_auth: false\n  self_serve_registration: false\n  dynamic_client_registration: false\n  api_key_program: false\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - https://www.wyndhambusiness.com/wp-json/wp/v2\n  - https://development.wyndhamhotels.com/wp-json/wp/v2\n  evidence: |\n    GET /wp-json/\
  \ returns HTTP 200 with \"authentication\":\n    {\"application-passwords\":{...}} only. Anonymous HTTP 200 confirmed on\n    /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags,\n    /wp/v2/users, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses,\n    /wp/v2/comments, /wp/v2/search and /wp/v2/blocks on www.wyndhambusiness.com.\n- name: wyndham-business-mcp-oauth\n  type: oauth2\n  applies_to:\n  - https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server\n  source: well-known/wyndham-hotels-wyndhambusiness-oauth-authorization-server.json\n  issuer: https://www.wyndhambusiness.com\n  authorization_server_metadata: https://www.wyndhambusiness.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://www.wyndhambusiness.com/.well-known/oauth-protected-resource\n  resource: https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wyndhambusiness.com/oauth/authorize\n\
  \    tokenUrl: https://www.wyndhambusiness.com/oauth/token\n    refreshUrl: https://www.wyndhambusiness.com/oauth/token\n    scopes:\n      mcp: Access the WordPress MCP server on www.wyndhambusiness.com\n  revocation_endpoint: https://www.wyndhambusiness.com/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  client_id_metadata_document_supported: true\n  registration_endpoint: null\n  bearer_methods_supported:\n  - header\n  client_credentials: false\n  evidence: |\n    Anonymous JSON-RPC tools/list returns 401 mcp_unauthorized with\n    WWW-Authenticate: Bearer realm=\"https://www.wyndhambusiness.com\",\n    resource_metadata=\"https://www.wyndhambusiness.com/.well-known/oauth-protected-resource\"\n  note: |\n    PKCE S256 is the only code-challenge method and the token endpoint accepts no\n    client authentication,\
  \ which is the OAuth 2.1 public-client profile the MCP\n    authorization spec expects. There is no registration endpoint; clients are\n    expected to present a client-id metadata document URL.\n- name: wordpress-privileged\n  type: cookie+nonce / application-password\n  applies_to:\n  - https://www.wyndhambusiness.com/wp-json/\n  - https://development.wyndhamhotels.com/wp-json/\n  public: false\n  application_passwords_endpoint: https://www.wyndhambusiness.com/wp-admin/authorize-application.php\n  evidence: |\n    GET /wp-json/wp/v2/settings returns 401 rest_forbidden;\n    GET /wp-json/wp-abilities/v1/abilities returns 401 rest_forbidden;\n    POST /wp-json/mcp/mcp-adapter-default-server returns 401 rest_forbidden.\n    CORS advertises Authorization and X-WP-Nonce in access-control-allow-headers.\n- name: human-login-walls\n  type: none-machine-readable\n  applies_to:\n  - https://www.wyndhambusiness.com/ (Wyndham Business account)\n  - https://www.wyndhamhotels.com/wyndham-rewards\
  \ (Wyndham Rewards member)\n  - https://wyndham.supplierone.co/ (supplier procurement, third party)\n  note: |\n    Human sign-in surfaces only. Wyndham Business / Wyndham Direct access is\n    approval-gated on a submitted request with a corporate code, company name,\n    website URL and anticipated travel spend; none of it produces an API credential.\ndocs: null\ndocs_note: |\n  Wyndham publishes no authentication documentation. The upstream semantics for the\n  WordPress surfaces are documented by WordPress, not by Wyndham:\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ncross_references:\n  scopes: scopes/wyndham-hotels-scopes.yml\n  well_known: well-known/wyndham-hotels-well-known.yml\n  mcp: mcp/wyndham-hotels-mcp.yml\n  conventions: conventions/wyndham-hotels-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyndham-hotels/refs/heads/main/authentication/wyndham-hotels-authentication.yml
summary_line: none/oauth2 · 4 schemes
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Franchising
- Distribution
- Loyalty
- GDS
---
