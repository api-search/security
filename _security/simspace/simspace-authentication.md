---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Simspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimSpace declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SimSpace
provider_slug: simspace
scheme_count: 2
schemes:
- applies_to: https://simspace.com/wp-json/mcp/mcp-oauth-server
  bearer_methods:
  - header
  challenge:
    rfc: RFC 9728
    status: 401
    www_authenticate: Bearer realm="https://simspace.com", resource_metadata="https://simspace.com/.well-known/oauth-protected-resource"
  client_registration: client_id_metadata_document_supported
  flows:
    authorizationCode:
      authorizationUrl: https://simspace.com/oauth/authorize
      refreshUrl: https://simspace.com/oauth/token
      revocationUrl: https://simspace.com/oauth/revoke
      scopes:
        mcp: Access the MCP server surface
      tokenUrl: https://simspace.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2-mcp
  pkce:
    methods:
    - S256
    required: unknown
  response_types:
  - code
  source: https://simspace.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
- applies_to: https://portal.simspace.com/api/v1
  documented: false
  name: platform-api-unknown
  note: Live host; an anonymous unparameterized request returns HTTP 400 "invalid arguments" rather than a 401, so no authentication challenge is emitted to unauthenticated callers and the scheme cannot be inferred. The API reference lives inside the authenticated portal SPA (portal.simspace.com/docs/latest/) and the customer-only Freshdesk support site.
  type: unknown
slug: simspace-authentication
source_filename: simspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://simspace.com/.well-known/oauth-authorization-server\nnote: >-\n  SimSpace publishes no public API authentication documentation. Everything recorded\n  here was observed directly on live hosts. The OAuth 2.0 profile below belongs to the\n  MCP surface on simspace.com, which is the only authentication surface SimSpace exposes\n  anonymously in machine-readable form. The platform API at portal.simspace.com/api/v1\n  and the portal SSO host portal-sso.simspace.com return 403 for every /.well-known/\n  path, so their auth scheme could not be established without credentials.\nschemes:\n- name: oauth2-mcp\n  type: oauth2\n  applies_to: https://simspace.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorizationCode:\n      authorizationUrl: https://simspace.com/oauth/authorize\n      tokenUrl: https://simspace.com/oauth/token\n      refreshUrl: https://simspace.com/oauth/token\n      revocationUrl: https://simspace.com/oauth/revoke\n\
  \      scopes:\n        mcp: Access the MCP server surface\n  pkce:\n    required: unknown\n    methods:\n    - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - none\n  client_registration: client_id_metadata_document_supported\n  bearer_methods:\n  - header\n  challenge:\n    status: 401\n    www_authenticate: Bearer realm=\"https://simspace.com\", resource_metadata=\"https://simspace.com/.well-known/oauth-protected-resource\"\n    rfc: RFC 9728\n  source: https://simspace.com/.well-known/oauth-authorization-server\n- name: platform-api-unknown\n  type: unknown\n  applies_to: https://portal.simspace.com/api/v1\n  documented: false\n  note: >-\n    Live host; an anonymous unparameterized request returns HTTP 400 \"invalid arguments\"\n    rather than a 401, so no authentication challenge is emitted to unauthenticated\n    callers and the scheme cannot be inferred. The API reference lives inside the\n    authenticated\
  \ portal SPA (portal.simspace.com/docs/latest/) and the customer-only\n    Freshdesk support site.\nidentity_providers:\n  sso_host: https://portal-sso.simspace.com/\n  protocols: unknown\n  note: A dedicated SSO host exists and is a tracked Statuspage component, but its\n    /.well-known/openid-configuration returns 403 so the protocol could not be confirmed.\nx-evidence:\n- url: https://simspace.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-27'\n- url: https://simspace.com/wp-json/mcp/mcp-oauth-server\n  http_status: 401\n  fetched: '2026-08-27'\n- url: https://portal.simspace.com/api/v1\n  http_status: 400\n  body: invalid arguments\n  fetched: '2026-08-27'\n- url: https://portal-sso.simspace.com/.well-known/openid-configuration\n  http_status: 403\n  fetched: '2026-08-27'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simspace/refs/heads/main/authentication/simspace-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cybersecurity
- Cyber Range
- Security Training
- Simulation
- AI Agents
- Security Operations
- Critical Infrastructure
- Government
- Compliance
---
