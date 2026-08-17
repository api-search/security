---
api_key_in: []
api_specs:
- filename: cello-events-api-openapi.yml
  format: yaml
  label: Cello Events API
  slug: cello-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-events-api-openapi.yml
- filename: cello-new-users-api-openapi.yml
  format: yaml
  label: Cello New Users API
  slug: cello-new-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-new-users-api-openapi.yml
- filename: cello-referral-codes-api-openapi.yml
  format: yaml
  label: Cello Referral Codes API
  slug: cello-referral-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referral-codes-api-openapi.yml
- filename: cello-referrers-api-openapi.yml
  format: yaml
  label: Cello Referrers API
  slug: cello-referrers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referrers-api-openapi.yml
- filename: cello-token-api-openapi.yml
  format: yaml
  label: Cello Token API
  slug: cello-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-token-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cello Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cello secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cello
provider_slug: cello
scheme_count: 3
schemes:
- credential_exchange:
    access_token_ttl_seconds: 18000
    endpoint: POST /token
    environment_scoped: true
    issued_from: Cello Portal -> Integrations -> Access Keys (https://portal.cello.so/integrations/accesskeys)
    refresh_fields:
    - refreshToken
    refresh_token_ttl_seconds: 432000
    request_fields:
    - accessKeyId
    - secretAccessKey
    response_fields:
    - accessToken
    - refreshToken
    - expiresIn
    - refreshTokenExpiresIn
    ttl_source: Published response examples in the OpenAPI (expiresIn 18000 = 5 hours, refreshTokenExpiresIn 432000 = 5 days).
    unauthenticated: true
  hosts:
  - https://api.cello.so
  - https://api.sandbox.cello.so
  name: bearerAuth
  scheme: bearer
  scopes: []
  sources:
  - openapi/cello-token-api-openapi.yml
  - openapi/cello-events-api-openapi.yml
  - openapi/cello-new-users-api-openapi.yml
  - openapi/cello-referral-codes-api-openapi.yml
  - openapi/cello-referrers-api-openapi.yml
  surface: rest
  type: http
- authorization_server: https://auth.cello.so
  discovery:
    authorization_server: https://auth.cello.so/.well-known/oauth-authorization-server
    protected_resource: https://mcp.cello.so/.well-known/oauth-protected-resource
  dynamic_client_registration: https://auth.cello.so/oauth2/register
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  - device_code
  hosts:
  - https://mcp.cello.so
  - https://mcp.sandbox.cello.so
  name: mcp-oauth
  note: Not declared in any OpenAPI — discovered by probing the MCP endpoint, which answers an unauthenticated tools/list with 401 and a WWW-Authenticate resource_metadata pointer.
  pkce: S256
  ref: ../scopes/cello-scopes.yml
  scopes:
  - mcp:read
  - mcp:write
  surface: mcp
  type: oauth2
- identifies: the end user, via productUserId
  name: component-jwt
  note: A product-signed JWT boots the Referral Component for a specific end user. It authenticates a user into the widget, not a server into the API, and is documented at https://docs.cello.so/sdk/client-side/user-authentication rather than in the API reference.
  signed_with: Product Secret (Cello Portal -> Integrations -> Access Keys)
  surface: embedded-components
  type: jwt
  used_by:
  - Cello JS (web Referral Component)
  - iOS / Android / React Native / Flutter SDKs
slug: cello-authentication
source_filename: cello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource:\n- https://docs.cello.so/api-reference/introduction\n- https://docs.cello.so/api-reference/authentication/get-token\n- https://mcp.cello.so/.well-known/oauth-protected-resource\n- https://auth.cello.so/.well-known/oauth-authorization-server\n- openapi/cello-token-api-openapi.yml\ndocs: https://docs.cello.so/api-reference/introduction\nsummary:\n  types:\n  - http\n  - oauth2\n  note: >-\n    Cello runs two independent authentication systems. The REST API uses a credential exchange —\n    POST /token with accessKeyId + secretAccessKey returns a short-lived bearer accessToken — and\n    declares only bearerAuth in the OpenAPI. The hosted MCP server uses full OAuth 2.0 against\n    https://auth.cello.so, with RFC 9728 protected-resource metadata, dynamic client registration\n    and PKCE. Neither system's credentials work on the other surface. A third mechanism, a\n    product-signed JWT, authenticates end users into the embedded\
  \ web and mobile components.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  surface: rest\n  hosts:\n  - https://api.cello.so\n  - https://api.sandbox.cello.so\n  credential_exchange:\n    endpoint: POST /token\n    unauthenticated: true\n    request_fields:\n    - accessKeyId\n    - secretAccessKey\n    refresh_fields:\n    - refreshToken\n    response_fields:\n    - accessToken\n    - refreshToken\n    - expiresIn\n    - refreshTokenExpiresIn\n    access_token_ttl_seconds: 18000\n    refresh_token_ttl_seconds: 432000\n    ttl_source: >-\n      Published response examples in the OpenAPI (expiresIn 18000 = 5 hours,\n      refreshTokenExpiresIn 432000 = 5 days).\n    issued_from: Cello Portal -> Integrations -> Access Keys (https://portal.cello.so/integrations/accesskeys)\n    environment_scoped: true\n  scopes: []\n  sources:\n  - openapi/cello-token-api-openapi.yml\n  - openapi/cello-events-api-openapi.yml\n  - openapi/cello-new-users-api-openapi.yml\n  - openapi/cello-referral-codes-api-openapi.yml\n\
  \  - openapi/cello-referrers-api-openapi.yml\n- name: mcp-oauth\n  type: oauth2\n  surface: mcp\n  hosts:\n  - https://mcp.cello.so\n  - https://mcp.sandbox.cello.so\n  authorization_server: https://auth.cello.so\n  flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - device_code\n  pkce: S256\n  dynamic_client_registration: https://auth.cello.so/oauth2/register\n  scopes:\n  - mcp:read\n  - mcp:write\n  discovery:\n    protected_resource: https://mcp.cello.so/.well-known/oauth-protected-resource\n    authorization_server: https://auth.cello.so/.well-known/oauth-authorization-server\n  ref: ../scopes/cello-scopes.yml\n  note: >-\n    Not declared in any OpenAPI — discovered by probing the MCP endpoint, which answers an\n    unauthenticated tools/list with 401 and a WWW-Authenticate resource_metadata pointer.\n- name: component-jwt\n  type: jwt\n  surface: embedded-components\n  signed_with: Product Secret (Cello Portal -> Integrations -> Access Keys)\n  identifies:\
  \ the end user, via productUserId\n  used_by:\n  - Cello JS (web Referral Component)\n  - iOS / Android / React Native / Flutter SDKs\n  note: >-\n    A product-signed JWT boots the Referral Component for a specific end user. It authenticates a\n    user into the widget, not a server into the API, and is documented at\n    https://docs.cello.so/sdk/client-side/user-authentication rather than in the API reference.\nobservations:\n- id: no-oauth-on-rest\n  detail: >-\n    The REST API publishes no OAuth metadata on api.cello.so — /.well-known/oauth-authorization-server\n    and /.well-known/openid-configuration both 404 — and the mcp:read / mcp:write scopes do not\n    apply to it. There is no scoped, least-privilege credential for the REST surface: an\n    accessToken is all-or-nothing across all six operations, including the destructive\n    POST /referrers/{productUserId}/depersonalize.\n- id: unauthenticated-401-shapes-differ\n  detail: >-\n    The two REST error envelopes disagree.\
  \ An unauthenticated resource call returns\n    {\"message\":\"Unauthorized\"}; a bad credential exchange at POST /token returns\n    {\"statusCode\":401,\"timestamp\":\"...\",\"path\":\"/api/token\",\"message\":\"Invalid API Credentials\"} —\n    a richer NestJS-style envelope, and one that leaks an internal path prefix (/api/token) the\n    public route does not use.\n  evidence:\n  - url: https://api.cello.so/referral-codes/TESTCODE123\n    status: 401\n  - url: https://api.cello.so/token\n    status: 401\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: 'https://docs.cello.so/api-reference/authentication/get-token.md', http_status: 200}\n  - {url: 'https://mcp.cello.so/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://auth.cello.so/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://api.cello.so/.well-known/oauth-authorization-server', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/authentication/cello-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- SaaS
- Attribution
- Partner Programs
- Ai Enterprise Software
---
