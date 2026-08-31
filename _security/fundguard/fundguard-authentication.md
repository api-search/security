---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Fundguard Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FundGuard secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FundGuard
provider_slug: fundguard
scheme_count: 1
schemes:
- client_registration:
    client_id_metadata_document_supported: true
    dynamic_client_registration: false
  flows:
  - authorizationUrl: https://www.fundguard.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refresh_supported: true
    revocationUrl: https://www.fundguard.com/oauth/revoke
    scopes:
      mcp: Access the FundGuard MCP server
    tokenUrl: https://www.fundguard.com/oauth/token
  issuer: https://www.fundguard.com
  name: mcp-oauth
  protected_resource: https://www.fundguard.com/wp-json/mcp/mcp-oauth-server
  sources:
  - well-known/fundguard-oauth-authorization-server.json
  - well-known/fundguard-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: fundguard-authentication
source_filename: fundguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://www.fundguard.com/.well-known/oauth-authorization-server\nnote: >-\n  FundGuard publishes no OpenAPI, so no securitySchemes could be derived. The only machine-readable\n  authentication contract FundGuard serves publicly is the RFC 8414 OAuth authorization-server metadata and\n  the RFC 9728 protected-resource metadata that front the MCP server on www.fundguard.com. The investment\n  accounting platform's own authentication model is not publicly documented; tenant logins live on per-tenant\n  hosts (login-<tenant>-eastus.fundguard.com, seen only in certificate transparency logs and not resolvable\n  from the public internet).\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  bearer_methods: [header]\n  pkce: [S256]\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  protected_resource: https://www.fundguard.com/wp-json/mcp/mcp-oauth-server\n  issuer: https://www.fundguard.com\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://www.fundguard.com/oauth/authorize\n    tokenUrl: https://www.fundguard.com/oauth/token\n    revocationUrl: https://www.fundguard.com/oauth/revoke\n    refresh_supported: true\n    pkce: S256\n    scopes:\n      mcp: Access the FundGuard MCP server\n  client_registration:\n    dynamic_client_registration: false\n    client_id_metadata_document_supported: true\n  token_endpoint_auth_methods: [none]\n  sources:\n  - well-known/fundguard-oauth-authorization-server.json\n  - well-known/fundguard-oauth-protected-resource.json\nundocumented:\n- surface: FundGuard investment accounting platform API\n  reason: >-\n    marketed as API-first for portfolio management, custodian, administrator and data-provider integration,\n    but no developer portal, API reference, or auth documentation is published on any public FundGuard host\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - https://www.fundguard.com/.well-known/oauth-authorization-server\n\
  \  - https://www.fundguard.com/.well-known/oauth-protected-resource\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundguard/refs/heads/main/authentication/fundguard-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- investment-accounting
- fund-accounting
- ibor
- abor
- nav
- asset-management
- portfolio-accounting
- private-markets
- Financial-Services
- Fintech
- saas
- artificial-intelligence
- MCP
---
