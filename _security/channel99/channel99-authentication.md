---
api_key_in:
- header
api_specs:
- filename: channel99-pulsar-openapi.json
  format: json
  label: Channel99 Pulsar Reporting API
  slug: channel99-pulsar-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-pulsar-openapi.json
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Channel99 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Channel99 secures its APIs with apiKey, http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Channel99
provider_slug: channel99
scheme_count: 4
schemes:
- api: Pulsar Reporting API
  bearerFormat: JWT
  description: 'M2M Bearer token issued by Stytch. Pass as `Authorization: Bearer <token>`.'
  name: bearerAuth
  rate_limit: 20 requests/minute per client_id on POST /auth/token (plus a WAF per-IP limit)
  refresh: No refresh token. Re-POST /auth/token to mint a new access token after expiry. The developer guide instructs callers to cache the token securely only for its stated lifetime.
  scheme: bearer
  sources:
  - openapi/channel99-pulsar-openapi.json
  - https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide
  token_endpoint: https://pulsar.channel99.com/auth/token
  token_lifetime_seconds: 3600
  token_request:
    body_fields:
    - client_id
    - client_secret
    content_type: application/json
    method: POST
  token_response_fields:
  - access_token
  - token_type
  - expires_in
  type: http
- api: Pulsar Reporting API
  description: 'Client identifier that must match the `client_id` claim in the Bearer token. Required on

    EVERY route including /openapi.json - omitting it returns HTTP 401

    err:pulsar.core.missing-header. A mismatch between the header and the token returns HTTP 403.'
  example_shape: m2m-client-00000000-0000-0000-0000-000000000000
  in: header
  name: clientId
  parameter: x-client-id
  required: true
  sources:
  - openapi/channel99-pulsar-openapi.json
  - https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide
  type: apiKey
- api: Channel99 MCP Server
  client_id_metadata_document_supported: true
  code_challenge_methods:
  - S256
  dynamic_client_registration: false
  flows:
    authorizationCode:
      authorizationUrl: https://app.channel99.com/oauth/authorize
      scopes:
        email: Read the authenticated user's email address
        openid: Authenticate the user and issue an ID token
        profile: Read the authenticated user's basic profile
      tokenUrl: https://api.stytch.app.channel99.com/v1/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  name: mcpOAuth
  pkce_required: true
  protected_resource: https://mcp.channel99.com
  sources:
  - well-known/channel99-mcp-oauth-authorization-server.json
  - well-known/channel99-mcp-oauth-protected-resource.json
  - https://support.channel99.com/hc/en-us/articles/47105598392475-MCP-Server-General-FAQ
  standard: OAuth 2.1
  token_endpoint_auth_methods:
  - none
  type: oauth2
- api: Channel99 web application
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://api.stytch.app.channel99.com
  jwks_uri: https://api.stytch.app.channel99.com/.well-known/jwks.json
  name: stytchOIDC
  openIdConnectUrl: https://api.stytch.app.channel99.com/.well-known/openid-configuration
  scopes_supported:
  - openid
  - profile
  - email
  - phone
  - offline_access
  - full_access
  sources:
  - well-known/channel99-stytch-openid-configuration.json
  sso: The app publishes /sign-in/sso and per-organization sign-in routes (/sign-in/inst/:orgSlug), so enterprise SSO is supported through Stytch B2B organizations.
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://api.stytch.app.channel99.com/v1/oauth2/userinfo
slug: channel99-authentication
source_filename: channel99-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide\ndocs:\n- https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide\n- https://pulsar.channel99.com/docs/#/\n- https://mcp.channel99.com/.well-known/oauth-authorization-server\nderived_from:\n- openapi/channel99-pulsar-openapi.json\n- well-known/channel99-mcp-oauth-authorization-server.json\n- well-known/channel99-mcp-oauth-protected-resource.json\n\nnote: >-\n  Channel99 runs two distinct authentication models. The Pulsar Reporting API uses a\n  machine-to-machine client_credentials exchange against its own /auth/token endpoint, returning\n  a short-lived Stytch-issued JWT that must be paired with a matching x-client-id header on\n  every request. The MCP server and the web application use interactive OAuth 2.1 /\n  OpenID Connect against a Stytch authorization server hosted on\
  \ a Channel99 subdomain.\n\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  credential_issuance: >-\n    Channel99 issues the M2M client_id and client_secret per customer instance; there is no\n    self-service key page. Credentials are bound to a single Channel99 instance, so a token can\n    only read data belonging to that tenant.\n\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  api: Pulsar Reporting API\n  description: |-\n    M2M Bearer token issued by Stytch. Pass as `Authorization: Bearer <token>`.\n  token_endpoint: https://pulsar.channel99.com/auth/token\n  token_request:\n    method: POST\n    content_type: application/json\n    body_fields:\n    - client_id\n    - client_secret\n  token_response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  token_lifetime_seconds: 3600\n  refresh: >-\n    No refresh token. Re-POST /auth/token to mint a new access token after expiry. The\n\
  \    developer guide instructs callers to cache the token securely only for its stated lifetime.\n  rate_limit: 20 requests/minute per client_id on POST /auth/token (plus a WAF per-IP limit)\n  sources:\n  - openapi/channel99-pulsar-openapi.json\n  - https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide\n\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: x-client-id\n  api: Pulsar Reporting API\n  required: true\n  description: |-\n    Client identifier that must match the `client_id` claim in the Bearer token. Required on\n    EVERY route including /openapi.json - omitting it returns HTTP 401\n    err:pulsar.core.missing-header. A mismatch between the header and the token returns HTTP 403.\n  example_shape: m2m-client-00000000-0000-0000-0000-000000000000\n  sources:\n  - openapi/channel99-pulsar-openapi.json\n  - https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide\n\n- name:\
  \ mcpOAuth\n  type: oauth2\n  api: Channel99 MCP Server\n  standard: OAuth 2.1\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.channel99.com/oauth/authorize\n      tokenUrl: https://api.stytch.app.channel99.com/v1/oauth2/token\n      scopes:\n        openid: Authenticate the user and issue an ID token\n        email: Read the authenticated user's email address\n        profile: Read the authenticated user's basic profile\n  pkce_required: true\n  code_challenge_methods:\n  - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  dynamic_client_registration: false\n  client_id_metadata_document_supported: true\n  protected_resource: https://mcp.channel99.com\n  sources:\n  - well-known/channel99-mcp-oauth-authorization-server.json\n  - well-known/channel99-mcp-oauth-protected-resource.json\n  - https://support.channel99.com/hc/en-us/articles/47105598392475-MCP-Server-General-FAQ\n\n- name: stytchOIDC\n  type: openIdConnect\n\
  \  api: Channel99 web application\n  openIdConnectUrl: https://api.stytch.app.channel99.com/.well-known/openid-configuration\n  issuer: https://api.stytch.app.channel99.com\n  jwks_uri: https://api.stytch.app.channel99.com/.well-known/jwks.json\n  userinfo_endpoint: https://api.stytch.app.channel99.com/v1/oauth2/userinfo\n  id_token_signing_alg_values_supported:\n  - RS256\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - phone\n  - offline_access\n  - full_access\n  subject_types_supported:\n  - public\n  sso: >-\n    The app publishes /sign-in/sso and per-organization sign-in routes\n    (/sign-in/inst/:orgSlug), so enterprise SSO is supported through Stytch B2B organizations.\n  sources:\n  - well-known/channel99-stytch-openid-configuration.json\n\nsecrets_handling:\n  guidance_published: true\n  guidance: >-\n    \"Store the client secret securely. Do not include client secrets or access tokens in emails,\n    support tickets, browser screenshots, logs, source control,\
  \ or client-side code.\" Support\n    tickets must exclude tokens and secrets.\n  source: https://support.channel99.com/hc/en-us/articles/49766041989787-Channel99-Reporting-API-Developer-Guide\n\nseparately_permissioned:\n- surface: Channel99 IP API (GET /ip/{ipAddress})\n  note: >-\n    \"Access to separately permissioned services, including the Channel99 IP API, is not enabled\n    unless explicitly granted.\" A valid token for the Reporting API does not imply access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/authentication/channel99-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Marketing
- Analytics
- Attribution
- B2B
- Advertising
- Marketing Technology
- Artificial Intelligence
- Account Based Marketing
- Reporting
- MCP
- Agent Ready
- Intent Data
- Account Identification
- Data Export
---
