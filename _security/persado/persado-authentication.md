---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Persado Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Persado secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Persado
provider_slug: persado
scheme_count: 2
schemes:
- applies_to: https://api.persado.com/mcp
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth
    flow: authorizationCode
    refreshUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token
    scopes:
      mcp:tools: Invoke tools exposed by the Persado MCP Gateway
      offline_access: Issue a refresh token for long-lived agent sessions
      openid: OpenID Connect authentication
    tokenUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://myaccount.persado.com/realms/persado-portal
  jwks_uri: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/certs
  name: PersadoMCPGatewayOAuth
  note: token_endpoint_auth_methods "none" plus S256-only PKCE means the gateway expects PUBLIC clients using PKCE — the current OAuth 2.1 / MCP best-practice shape for agent clients, not a weakness.
  registration_endpoint: https://api.persado.com/register
  registration_spec: RFC 7591 dynamic client registration
  response_types_supported:
  - code
  source: https://api.persado.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: https://myaccount.persado.com/realms/persado-portal
  code_challenge_methods_supported:
  - plain
  - S256
  endpoints:
    authorization: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth
    device_authorization: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth/device
    end_session: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/logout
    introspection: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token/introspect
    jwks: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/certs
    registration: https://myaccount.persado.com/realms/persado-portal/clients-registrations/openid-connect
    revocation: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/revoke
    token: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token
    userinfo: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  issuer: https://myaccount.persado.com/realms/persado-portal
  name: PersadoPortalKeycloakOIDC
  note: Stock Keycloak realm surface. Includes mutual-TLS client authentication (tls_client_auth) and private_key_jwt, both available to enterprise integrations. The MCP gateway does not use these.
  openIdConnectUrl: https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration
  source: https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
slug: persado-authentication
source_filename: persado-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.persado.com/.well-known/oauth-authorization-server,\n  https://api.persado.com/.well-known/oauth-protected-resource,\n  https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\nnotes: >-\n  Persado publishes no OpenAPI, so this profile is not derived from a spec. It\n  is transcribed from three machine-readable discovery documents Persado itself\n  serves: the RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata on api.persado.com, and the full OpenID Connect\n  discovery document for the Keycloak realm persado-portal on\n  myaccount.persado.com. Nothing here is inferred from marketing copy.\n  Two distinct scope sets are recorded deliberately. The MCP gateway advertises\n  a narrow, deliberately-scoped set (openid, offline_access, mcp:tools) and\n  restricts itself to authorization_code + refresh_token with mandatory PKCE\n  S256 and public clients.\
  \ The underlying Keycloak realm advertises the full\n  stock Keycloak surface (13 scopes, 10 grant types including implicit and\n  password, and plain PKCE). The gateway's narrower profile is the one that\n  governs agent access, and it is the stronger of the two.\n\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  pkce_required: true\n  pkce_methods:\n  - S256\n  bearer_methods:\n  - header\n  dynamic_client_registration: true\n  public_clients: true\n\nschemes:\n- name: PersadoMCPGatewayOAuth\n  type: oauth2\n  applies_to: https://api.persado.com/mcp\n  source: https://api.persado.com/.well-known/oauth-authorization-server\n  issuer: https://myaccount.persado.com/realms/persado-portal\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth\n    tokenUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token\n\
  \    refreshUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token\n    scopes:\n      openid: OpenID Connect authentication\n      offline_access: Issue a refresh token for long-lived agent sessions\n      mcp:tools: Invoke tools exposed by the Persado MCP Gateway\n  jwks_uri: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/certs\n  registration_endpoint: https://api.persado.com/register\n  registration_spec: RFC 7591 dynamic client registration\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  note: >-\n    token_endpoint_auth_methods \"none\" plus S256-only PKCE means the gateway\n    expects PUBLIC clients using PKCE — the current OAuth 2.1 / MCP\n    best-practice shape for agent clients, not a weakness.\n\n- name: PersadoPortalKeycloakOIDC\n  type: openIdConnect\n\
  \  applies_to: https://myaccount.persado.com/realms/persado-portal\n  source: https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\n  openIdConnectUrl: https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\n  issuer: https://myaccount.persado.com/realms/persado-portal\n  endpoints:\n    authorization: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth\n    token: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token\n    userinfo: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/userinfo\n    jwks: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/certs\n    introspection: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token/introspect\n    revocation: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/revoke\n    end_session: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/logout\n\
  \    device_authorization: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth/device\n    registration: https://myaccount.persado.com/realms/persado-portal/clients-registrations/openid-connect\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  note: >-\n    Stock Keycloak realm surface. Includes mutual-TLS client authentication\n    (tls_client_auth) and private_key_jwt, both available to enterprise\n    integrations. The MCP gateway does\
  \ not use these.\n\nundocumented:\n  developer_docs: >-\n    Persado publishes no public authentication documentation, no developer\n    portal and no API reference. Everything above was read from discovery\n    documents, not from prose. A provider-published auth guide would be the\n    single highest-value addition to this surface.\n  legacy_enterprise_api: >-\n    Persado's platform pages describe a \"Lite API\", server-side API\n    integration and a client-side JavaScript snippet, and the persado/\n    GitHub org ships an Enterprise API Mobile SDK, but the authentication\n    model for that older Enterprise API is not published anywhere public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persado/refs/heads/main/authentication/persado-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Ai Apps
- Artificial Intelligence
- Generative AI
- Marketing
- Customer Engagement
- Content Generation
- Personalization
- Agents
- MCP
- Compliance
- Financial Services
---
