---
api_key_in: []
api_specs:
- filename: skai-kenshoo-api-openapi.yml
  format: yaml
  label: Skai (Kenshoo) API
  slug: skai-kenshoo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skai-kenshoo/refs/heads/main/openapi/skai-kenshoo-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Skai Kenshoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skai (Kenshoo) declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Skai (Kenshoo)
provider_slug: skai-kenshoo
scheme_count: 5
schemes:
- applies_to: REST API (https://services.kenshoo.com)
  bearer_format: JWT
  declared_in_spec: true
  defined_in_spec: false
  description: 'Every REST call carries `Authorization: Bearer <access_token>`. The access token is a JWT issued by the Skai login server; it is short-lived and carries agency/role context.'
  header: Authorization
  id: BearerAuth
  in: header
  scheme: bearer
  type: http
- applies_to: REST API token issuance
  description: 'Not OAuth 2.0. A bespoke refresh-token grant: the developer generates a permanent refresh token plus client ID once, by logging in at https://login.kenshoo.com/api/dev/refresh-token, then exchanges it for access tokens.'
  id: SkaiRefreshTokenExchange
  method: POST
  operation_id: getAccessToken
  operational_note: Skai advises reusing an access token until `expires_in` elapses, because minting new tokens too often trips the rate limit. Expiry is detected either by tracking `expires_in` or by handling HTTP 401.
  parameters:
  - location: body
    name: refresh_token
    note: Permanent — does not expire. Skai explicitly rejects refresh tokens sent as URL query parameters; they must be in the POST body.
    required: true
  - location: body
    name: client_id
    required: true
  - location: body
    name: agency_id
    note: Required when the API user is assigned to multiple agencies, to pin the token context.
    required: false
  request_encoding: application/x-www-form-urlencoded
  response_fields:
  - access_token
  - expires_in
  - email
  token_endpoint: https://services.kenshoo.com/api/v1/token
  type: custom
  typical_expires_in_seconds: 21600
- applies_to: MCP servers (https://mcp.kenshoo.com)
  authorization_endpoint: https://auth0.kenshoo.com/authorize
  description: Standards-compliant OAuth 2.0 with RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, used by MCP clients (ChatGPT, Claude) that perform dynamic discovery.
  discovery:
    authorization_server_metadata: https://login.kenshoo.com/.well-known/oauth-authorization-server
    openid_configuration: null
    openid_configuration_note: /.well-known/openid-configuration returns 404 on login.kenshoo.com even though the `openid` scope is advertised — the OIDC discovery document is not published.
    protected_resource_metadata: https://mcp.kenshoo.com/.well-known/oauth-protected-resource
  grant_types:
  - authorization_code
  - refresh_token
  id: SkaiPlatformOAuth2
  issuer: https://login.kenshoo.com
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - profile
  - offline_access
  token_endpoint: https://login.kenshoo.com/api/oauth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
- applies_to: MCP servers, all clients except ChatGPT
  companion_header: ks-name
  description: 'A Personal Access Token distinct from the REST bearer token. Sent as `Authorization: Bearer <PAT>` together with a `ks-name` header identifying the Skai account. ChatGPT does not support header-based tokens, so OAuth is the only path there.'
  header: Authorization
  id: SkaiMCPPersonalAccessToken
  in: header
  issue_url: https://login.kenshoo.com/api/dev/refresh-token
  rotation_days: 90
  scheme_prefix: Bearer
  type: apiKey
- applies_to: skai.io WordPress MCP adapter (marketing site, not the platform)
  authorization_endpoint: https://skai.io/oauth/authorize
  client_id_metadata_document_supported: true
  discovery:
    authorization_server_metadata: https://skai.io/.well-known/oauth-authorization-server
  grant_types:
  - authorization_code
  - refresh_token
  id: SkaiSiteMCPOAuth
  issuer: https://skai.io
  pkce:
  - S256
  revocation_endpoint: https://skai.io/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://skai.io/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: skai-kenshoo-authentication
source_filename: skai-kenshoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://developers.skai.io/ (Authentication section of the Skai OpenAPI info.description),\n  https://login.kenshoo.com/.well-known/oauth-authorization-server,\n  https://mcp.kenshoo.com/.well-known/oauth-protected-resource,\n  https://skai-mcp-guide.vercel.app/\ndocs: https://developers.skai.io/\nsummary: >-\n  Two distinct auth models. The REST API uses a non-standard, long-lived refresh token\n  exchanged at a plain form-POST token endpoint for a short-lived JWT bearer access token.\n  The hosted MCP servers use standards-track OAuth 2.0 (RFC 8414 + RFC 9728 discovery,\n  authorization_code with PKCE S256) or a 90-day Personal Access Token in the Authorization\n  header.\nspec_defect:\n  finding: >-\n    The published OpenAPI declares a root-level `security: [{BearerAuth: []}]` but\n    `components.securitySchemes` is ABSENT — the scheme BearerAuth is referenced and never\n    defined. The contract is therefore not\
  \ machine-resolvable for auth, and generated clients\n    cannot know the scheme is HTTP bearer with a JWT. Captured as a fix in\n    overlays/skai-kenshoo-api-security-overlay.yaml.\n  source: openapi/skai-kenshoo-api-openapi.yml\nschemes:\n- id: BearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  applies_to: REST API (https://services.kenshoo.com)\n  declared_in_spec: true\n  defined_in_spec: false\n  description: >-\n    Every REST call carries `Authorization: Bearer <access_token>`. The access token is a JWT\n    issued by the Skai login server; it is short-lived and carries agency/role context.\n- id: SkaiRefreshTokenExchange\n  type: custom\n  applies_to: REST API token issuance\n  token_endpoint: https://services.kenshoo.com/api/v1/token\n  operation_id: getAccessToken\n  method: POST\n  request_encoding: application/x-www-form-urlencoded\n  parameters:\n  - name: refresh_token\n    required: true\n    location: body\n    note:\
  \ >-\n      Permanent — does not expire. Skai explicitly rejects refresh tokens sent as URL query\n      parameters; they must be in the POST body.\n  - name: client_id\n    required: true\n    location: body\n  - name: agency_id\n    required: false\n    location: body\n    note: Required when the API user is assigned to multiple agencies, to pin the token context.\n  response_fields: [access_token, expires_in, email]\n  typical_expires_in_seconds: 21600\n  description: >-\n    Not OAuth 2.0. A bespoke refresh-token grant: the developer generates a permanent refresh\n    token plus client ID once, by logging in at\n    https://login.kenshoo.com/api/dev/refresh-token, then exchanges it for access tokens.\n  operational_note: >-\n    Skai advises reusing an access token until `expires_in` elapses, because minting new\n    tokens too often trips the rate limit. Expiry is detected either by tracking `expires_in`\n    or by handling HTTP 401.\n- id: SkaiPlatformOAuth2\n  type: oauth2\n  applies_to:\
  \ MCP servers (https://mcp.kenshoo.com)\n  issuer: https://login.kenshoo.com\n  authorization_endpoint: https://auth0.kenshoo.com/authorize\n  token_endpoint: https://login.kenshoo.com/api/oauth/token\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_post, none]\n  scopes: [openid, email, profile, offline_access]\n  discovery:\n    authorization_server_metadata: https://login.kenshoo.com/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://mcp.kenshoo.com/.well-known/oauth-protected-resource\n    openid_configuration: null\n    openid_configuration_note: >-\n      /.well-known/openid-configuration returns 404 on login.kenshoo.com even though the\n      `openid` scope is advertised — the OIDC discovery document is not published.\n  description: >-\n    Standards-compliant OAuth 2.0 with RFC 8414 authorization-server metadata and RFC 9728\n    protected-resource metadata,\
  \ used by MCP clients (ChatGPT, Claude) that perform dynamic\n    discovery.\n- id: SkaiMCPPersonalAccessToken\n  type: apiKey\n  in: header\n  header: Authorization\n  scheme_prefix: Bearer\n  companion_header: ks-name\n  applies_to: MCP servers, all clients except ChatGPT\n  issue_url: https://login.kenshoo.com/api/dev/refresh-token\n  rotation_days: 90\n  description: >-\n    A Personal Access Token distinct from the REST bearer token. Sent as\n    `Authorization: Bearer <PAT>` together with a `ks-name` header identifying the Skai\n    account. ChatGPT does not support header-based tokens, so OAuth is the only path there.\n- id: SkaiSiteMCPOAuth\n  type: oauth2\n  applies_to: skai.io WordPress MCP adapter (marketing site, not the platform)\n  issuer: https://skai.io\n  authorization_endpoint: https://skai.io/oauth/authorize\n  token_endpoint: https://skai.io/oauth/token\n  revocation_endpoint: https://skai.io/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  pkce:\
  \ [S256]\n  scopes: [mcp]\n  token_endpoint_auth_methods: [none]\n  client_id_metadata_document_supported: true\n  discovery:\n    authorization_server_metadata: https://skai.io/.well-known/oauth-authorization-server\nidentity_scoping:\n  ks_name:\n    description: >-\n      Nearly every REST operation and every MCP session is scoped by a Skai account\n      identifier — the \"KS\" or ks name (e.g. ks1234), found in the Skai platform under\n      Administration -> About Skai -> Server ID. It is a query parameter (`ks`) on REST and a\n      header (`ks-name`) or URL path segment on MCP.\n  agency_id:\n    description: >-\n      Multi-agency users must pin an agency context at token-exchange time; the resulting\n      access token is valid only for that agency.\n  minimum_role: >-\n    API access requires a Skai user with the Standard role or higher. Skai recommends\n    creating a dedicated service user for API requests.\nmtls: false\nopenid_connect: false\nopenid_connect_note: >-\n  The\
  \ `openid` scope is advertised on the MCP authorization server, but no OIDC discovery\n  document is published, so OIDC cannot be claimed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skai-kenshoo/refs/heads/main/authentication/skai-kenshoo-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Commerce
- Advertising
- Marketing
- Retail Media
- Paid Search
- Paid Social
- Marketing Analytics
- Advertising Technology
- Campaign Management
- Commerce Media
- Reporting
- MCP
- agent-native
- Omnichannel
---
