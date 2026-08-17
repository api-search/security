---
api_key_in:
- header
api_specs:
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
- filename: rocketreach-company-data-api-api-openapi.yml
  format: yaml
  label: RocketReach Company Data API API
  slug: rocketreach-company-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-data-api-api-openapi.yml
- filename: rocketreach-people-data-api-api-openapi.yml
  format: yaml
  label: RocketReach People Data API API
  slug: rocketreach-people-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-data-api-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rocketreach Authentication
name_suffix: Authentication
oauth_flows: []
overview: RocketReach secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RocketReach
provider_slug: rocketreach
scheme_count: 2
schemes:
- applies_to: all 16 REST operations on https://api.rocketreach.co/api/v2
  description: RocketReach account API key. Locate it in the "My API Key" section of the API account page (https://rocketreach.co/account?section=nav_gen_api). Requests are authenticated with the Api-Key request header. Older clients may use an api_key query parameter, but that behaviour is deprecated.
  in: header
  name: RocketReachAPIKey
  parameter: Api-Key
  rotation:
    note: Minting a new key through the API returns it in an APIKey object; there is no published key-expiry policy.
    operation: create_new_api_key (POST /account/key/)
    self_service: true
  scopes: null
  sources:
  - openapi/_original/rocketreach-api-openapi.json
  - openapi/rocketreach-account-api-openapi.yml
  - openapi/rocketreach-company-data-api-api-openapi.yml
  - openapi/rocketreach-people-data-api-api-openapi.yml
  surface: rest
  type: apiKey
- applies_to: https://mcp.rocketreach.co/mcp
  client_responsibilities:
  - Generate and verify a random state parameter — CSRF defence is the client's job, not the server's.
  - redirect_uri must exactly match one bound at registration; non-localhost redirects must be https.
  - http://localhost and http://127.0.0.1 on any port are permitted for native/desktop clients (RFC 8252).
  description: OAuth 2.1 authorization-code flow with PKCE (S256) and open Dynamic Client Registration, protecting the hosted MCP server. MCP-compatible clients complete the flow automatically from the server URL.
  discovery:
    authorization_server: https://rocketreach.co/.well-known/oauth-authorization-server
    protected_resource: https://mcp.rocketreach.co/.well-known/oauth-protected-resource
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://rocketreach.co/mcp-oauth/authorize
      refreshUrl: https://rocketreach.co/mcp-oauth/token
      registrationUrl: https://rocketreach.co/mcp-oauth/register
      revocationUrl: https://rocketreach.co/mcp-oauth/revoke
      scopes:
        rocketreach:read: Access to all RocketReach MCP tools — search, lookup and account.
      tokenUrl: https://rocketreach.co/mcp-oauth/token
  name: RocketReachMCPOAuth
  pkce: S256
  scopes_detail: scopes/rocketreach-scopes.yml
  sources:
  - https://rocketreach.co/.well-known/oauth-authorization-server
  - https://docs.rocketreach.co/reference/mcp-auth
  surface: mcp
  token:
    access_token_lifetime: 1 hour
    audience_binding: bound to the MCP server URL; rejected by any other audience
    format: JWE-wrapped JWT — AES-256-GCM envelope over an HS256-signed JWS carrying sub, aud, exp and the account API key
    header: 'Authorization: Bearer <token>'
    refresh_rotation: single-use; replay revokes every token for that user+client
    refresh_token_lifetime: 30 days
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  version: '2.1'
slug: rocketreach-authentication
source_filename: rocketreach-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.rocketreach.co/reference/rocketreach-api, https://docs.rocketreach.co/reference/mcp-auth,\n  https://rocketreach.co/.well-known/oauth-authorization-server, openapi/_original/rocketreach-api-openapi.json\ndocs:\n- https://docs.rocketreach.co/reference/rocketreach-api\n- https://docs.rocketreach.co/reference/mcp-auth\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    RocketReach runs TWO distinct auth models on two distinct surfaces. The REST API at api.rocketreach.co is\n    API-key only. The MCP server at mcp.rocketreach.co is OAuth 2.1 with PKCE and Dynamic Client Registration.\n    An earlier round of this profile recorded only the API key, because the OpenAPI declares only the apiKey\n    scheme; the OAuth surface was found by probing /.well-known/oauth-authorization-server.\nschemes:\n- name: RocketReachAPIKey\n  surface: rest\n  type: apiKey\n  in: header\n  parameter:\
  \ Api-Key\n  description: >-\n    RocketReach account API key. Locate it in the \"My API Key\" section of the API account page\n    (https://rocketreach.co/account?section=nav_gen_api). Requests are authenticated with the Api-Key request\n    header. Older clients may use an api_key query parameter, but that behaviour is deprecated.\n  applies_to: all 16 REST operations on https://api.rocketreach.co/api/v2\n  rotation:\n    self_service: true\n    operation: create_new_api_key (POST /account/key/)\n    note: Minting a new key through the API returns it in an APIKey object; there is no published key-expiry policy.\n  scopes: null\n  sources:\n  - openapi/_original/rocketreach-api-openapi.json\n  - openapi/rocketreach-account-api-openapi.yml\n  - openapi/rocketreach-company-data-api-api-openapi.yml\n  - openapi/rocketreach-people-data-api-api-openapi.yml\n- name: RocketReachMCPOAuth\n  surface: mcp\n  type: oauth2\n  version: '2.1'\n  description: >-\n    OAuth 2.1 authorization-code flow\
  \ with PKCE (S256) and open Dynamic Client Registration, protecting the\n    hosted MCP server. MCP-compatible clients complete the flow automatically from the server URL.\n  applies_to: https://mcp.rocketreach.co/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://rocketreach.co/mcp-oauth/authorize\n      tokenUrl: https://rocketreach.co/mcp-oauth/token\n      refreshUrl: https://rocketreach.co/mcp-oauth/token\n      registrationUrl: https://rocketreach.co/mcp-oauth/register\n      revocationUrl: https://rocketreach.co/mcp-oauth/revoke\n      scopes:\n        rocketreach:read: Access to all RocketReach MCP tools — search, lookup and account.\n  pkce: S256\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported:\n  - none\n  token:\n    header: 'Authorization: Bearer <token>'\n    format: JWE-wrapped JWT — AES-256-GCM envelope over an HS256-signed JWS carrying sub, aud, exp and the account API key\n    access_token_lifetime: 1 hour\n    refresh_token_lifetime:\
  \ 30 days\n    refresh_rotation: single-use; replay revokes every token for that user+client\n    audience_binding: bound to the MCP server URL; rejected by any other audience\n  discovery:\n    protected_resource: https://mcp.rocketreach.co/.well-known/oauth-protected-resource\n    authorization_server: https://rocketreach.co/.well-known/oauth-authorization-server\n  client_responsibilities:\n  - Generate and verify a random state parameter — CSRF defence is the client's job, not the server's.\n  - redirect_uri must exactly match one bound at registration; non-localhost redirects must be https.\n  - http://localhost and http://127.0.0.1 on any port are permitted for native/desktop clients (RFC 8252).\n  scopes_detail: scopes/rocketreach-scopes.yml\n  sources:\n  - https://rocketreach.co/.well-known/oauth-authorization-server\n  - https://docs.rocketreach.co/reference/mcp-auth\nerrors:\n- surface: rest\n  status: 401\n  meaning: API key missing or invalid.\n- surface: rest\n  status: 403\n\
  \  meaning: API key lacks permission for the action.\n- surface: mcp\n  error: auth_required\n  status: 401\n  meaning: No Bearer token, expired token, wrong audience, or the account state (unverified email, suspended, region) blocked the call.\n- surface: mcp\n  error: invalid_scope\n  status: 400\n  meaning: A scope other than rocketreach:read (or empty) was requested.\ntransport_security:\n  https_required: true\n  hsts: true\n  detail: security/rocketreach-domain-security.yml\nmtls: false\nopenid_connect: false\nopenid_connect_note: /.well-known/openid-configuration returns 404 on every RocketReach host — OAuth here is authorization only, not identity.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/authentication/rocketreach-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
---
