---
api_key_in: []
auth_types: []
description: 'SocialBee publishes exactly one machine-readable authentication surface: an RFC 8414 OAuth 2.0 Authorization Server Metadata document at socialbee.com/.well-known/oauth-authorization-server. It guards the MCP server at socialbee.com/wp-json/mcp/mcp-oauth-server. The SocialBee product API at app.socialbee.com is not public and publishes no authentication documentation.'
kind: authentication
layout: security
method: probed
name: Socialbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: SocialBee declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SocialBee
provider_slug: socialbee
scheme_count: 1
schemes:
- authorization_endpoint: https://socialbee.com/oauth/authorize
  bearer_methods_supported:
  - header
  bearer_placement: 'Authorization: Bearer <token>'
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_registration: false
    note: No RFC 7591 registration_endpoint. Clients identify themselves with a Client ID Metadata Document — an HTTPS client_id URL that resolves to the client's own metadata.
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.1 authorization code flow with mandatory PKCE, protecting the MCP server. Public clients only — the token endpoint advertises auth method "none", so there is no client secret.
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: socialbee_oauth_mcp
  issuer: https://socialbee.com
  pkce_required: true
  protected_resources:
  - https://socialbee.com/wp-json/mcp/mcp-oauth-server
  response_types_supported:
  - code
  revocation_endpoint: https://socialbee.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://socialbee.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: socialbee-authentication
source_filename: socialbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://socialbee.com/.well-known/oauth-authorization-server\nname: SocialBee Authentication Profile\ndescription: >-\n  SocialBee publishes exactly one machine-readable authentication surface: an\n  RFC 8414 OAuth 2.0 Authorization Server Metadata document at\n  socialbee.com/.well-known/oauth-authorization-server. It guards the MCP server\n  at socialbee.com/wp-json/mcp/mcp-oauth-server. The SocialBee product API at\n  app.socialbee.com is not public and publishes no authentication documentation.\n\nschemes:\n  - id: socialbee_oauth_mcp\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      OAuth 2.1 authorization code flow with mandatory PKCE, protecting the MCP\n      server. Public clients only — the token endpoint advertises auth method\n      \"none\", so there is no client secret.\n    issuer: https://socialbee.com\n    authorization_endpoint: https://socialbee.com/oauth/authorize\n    token_endpoint:\
  \ https://socialbee.com/oauth/token\n    revocation_endpoint: https://socialbee.com/oauth/revoke\n    response_types_supported:\n      - code\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    code_challenge_methods_supported:\n      - S256\n    pkce_required: true\n    token_endpoint_auth_methods_supported:\n      - none\n    scopes:\n      - mcp\n    bearer_methods_supported:\n      - header\n    bearer_placement: 'Authorization: Bearer <token>'\n    client_registration:\n      dynamic_registration: false\n      client_id_metadata_document_supported: true\n      note: >-\n        No RFC 7591 registration_endpoint. Clients identify themselves with a\n        Client ID Metadata Document — an HTTPS client_id URL that resolves to the\n        client's own metadata.\n    protected_resources:\n      - https://socialbee.com/wp-json/mcp/mcp-oauth-server\n\nunauthenticated_error:\n  observed: true\n  http_status: 401\n  content_type: application/json\n  body:\
  \ '{\"code\":\"mcp_unauthorized\",\"message\":\"MCP authentication required.\",\"data\":{\"status\":401}}'\n  note: >-\n    Observed on an anonymous JSON-RPC POST to the MCP endpoint. The response is a\n    JSON error envelope, not RFC 9457 problem+json.\n\nproduct_api:\n  public: false\n  host: app.socialbee.com\n  note: >-\n    app.socialbee.com and api.socialbee.com both exist and both require a session\n    login (api.socialbee.com returns an HTML page titled \"API | Login into\n    SocialBee\" for every path, including /openapi.json). SocialBee's help centre\n    states there is no public REST API. End-user automation is brokered through\n    Zapier, Make and Pabbly connectors, which hold the credentials themselves, so\n    no SocialBee auth scheme is exposed to the integrator.\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - url: https://socialbee.com/.well-known/oauth-authorization-server\n      http_status: 200\n      content_type: application/json\n    - url: https://socialbee.com/wp-json/mcp/mcp-oauth-server\n\
  \      http_status: 401\n      note: anonymous JSON-RPC tools/list\n    - url: https://api.socialbee.com/openapi.json\n      http_status: 200\n      note: >-\n        HTML login shell titled \"API | Login into SocialBee\", NOT an OpenAPI\n        document. Recorded so a future run does not re-trip on this soft 200.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialbee/refs/heads/main/authentication/socialbee-authentication.yml
summary_line: 1 scheme
tags:
- Social Media Management
- Content Scheduling
- Content Recycling
- Social Media Analytics
- AI Caption Generation
- Social Media Publishing
- MCP
- Marketing Automation
- Software-as-a-Service
---
