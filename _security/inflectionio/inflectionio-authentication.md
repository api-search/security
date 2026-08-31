---
api_key_in: []
api_specs:
- filename: inflectionio-contact-activity-api-openapi.yml
  format: yaml
  label: Inflection.io Contact Activity API
  slug: inflectionio-contact-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contact-activity-api-openapi.yml
- filename: inflectionio-contacts-api-openapi.yml
  format: yaml
  label: Inflection.io Contacts API
  slug: inflectionio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contacts-api-openapi.yml
- filename: inflectionio-emails-api-openapi.yml
  format: yaml
  label: Inflection.io Emails API
  slug: inflectionio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-emails-api-openapi.yml
- filename: inflectionio-email-versions-api-openapi.yml
  format: yaml
  label: Inflection.io Email Versions API
  slug: inflectionio-email-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-email-versions-api-openapi.yml
- filename: inflectionio-lists-and-members-api-openapi.yml
  format: yaml
  label: Inflection.io Lists and Members API
  slug: inflectionio-lists-and-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-lists-and-members-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Inflectionio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Inflection.io secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Inflection.io
provider_slug: inflectionio
scheme_count: 2
schemes:
- applies_to:
  - https://api.inflection.io/v1
  best_practice: one token per integration so a single revoke does not break the others
  description: 'Personal Access Token or OAuth 2.1 access token sent as a bearer credential (Authorization: Bearer <token>). PATs are scoped READ (required for every GET) and WRITE (required for POST/PATCH/DELETE); OAuth tokens act as the user who authorized the app.'
  issuance: Inflection dashboard, Settings > Connected Apps > Personal Access Tokens > Create app credentials
  lifetime: long-lived, valid until revoked
  name: bearerAuth
  not_valid_for:
  - https://mcp.inflection.io/ — PATs explicitly do NOT work for MCP; MCP clients use a connected app's OAuth flow.
  permissions:
  - description: Required for every GET request.
    name: READ
  - description: Required for POST, PATCH, and DELETE requests.
    name: WRITE
  scheme: bearer
  shown_once: true
  sources:
  - openapi/_original/inflectionio-openapi-original.yml
  - https://docs.inflection.io/api-reference/get-your-pat
  token_prefix: inf_pat_
  type: http
- applies_to:
  - https://api.inflection.io/v1
  - https://mcp.inflection.io/
  - https://campaign.inflection.io/api/v1
  authorization_code_ttl_seconds: 300
  authorization_model: Acts as the user who authorized the app — workspace admins and members read and write, viewers are read-only. There is no client-credentials grant; service-to-service tokens are rejected with 403.
  client_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  description: OAuth 2.1 with PKCE (S256 required, plain rejected) for multi-user apps, automation platforms and any client that should not hold a long-lived secret. The same access token works on the Developer API and on the MCP server.
  discovery:
    authorization_server_metadata: https://auth-v2.inflection.io/.well-known/oauth-authorization-server
    protected_resource_metadata: https://mcp.inflection.io/.well-known/oauth-protected-resource
    specs:
    - RFC 8414
    - RFC 9728
  flows:
  - authorizationUrl: https://auth-v2.inflection.io/oauth2/authorize
    flow: authorizationCode
    introspectionUrl: https://auth-v2.inflection.io/oauth2/introspect
    jwksUri: https://auth-v2.inflection.io/oauth2/jwks
    registrationUrl: https://auth-v2.inflection.io/client-app/connect/register
    revocationUrl: https://auth-v2.inflection.io/oauth2/revoke
    scopes:
    - inflection_app
    tokenUrl: https://auth-v2.inflection.io/oauth2/token
  name: OAuth 2.1 Connected App
  refresh: refresh_token grant with rotation and reuse detection
  see: scopes/inflectionio-scopes.yml
  sources:
  - https://docs.inflection.io/agents/connected-apps-oauth
  - https://auth-v2.inflection.io/.well-known/oauth-authorization-server
  token_lifetime_seconds: 900
  type: oauth2
slug: inflectionio-authentication
source_filename: inflectionio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.inflection.io/api-reference/authentication\ndocs: https://docs.inflection.io/api-reference/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  token_types:\n  - personal-access-token\n  - oauth2-access-token\n  token_prefix: inf_pat_\n  permissions:\n  - READ\n  - WRITE\n  oauth2_scopes:\n  - inflection_app\n  note: >-\n    The OpenAPI declares only the http/bearer scheme. OAuth 2.1 is real and documented but invisible in\n    the spec — it is captured here from the docs and from live RFC 8414 / RFC 9728 discovery documents.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Personal Access Token or OAuth 2.1 access token sent as a bearer credential\n    (Authorization: Bearer <token>). PATs are scoped READ (required for every GET) and WRITE (required\n    for POST/PATCH/DELETE); OAuth tokens act as the\
  \ user who authorized the app.\n  token_prefix: inf_pat_\n  issuance: Inflection dashboard, Settings > Connected Apps > Personal Access Tokens > Create app credentials\n  lifetime: long-lived, valid until revoked\n  shown_once: true\n  best_practice: one token per integration so a single revoke does not break the others\n  permissions:\n  - name: READ\n    description: Required for every GET request.\n  - name: WRITE\n    description: Required for POST, PATCH, and DELETE requests.\n  applies_to: [https://api.inflection.io/v1]\n  not_valid_for:\n  - https://mcp.inflection.io/ — PATs explicitly do NOT work for MCP; MCP clients use a connected app's OAuth flow.\n  sources:\n  - openapi/_original/inflectionio-openapi-original.yml\n  - https://docs.inflection.io/api-reference/get-your-pat\n- name: OAuth 2.1 Connected App\n  type: oauth2\n  description: >-\n    OAuth 2.1 with PKCE (S256 required, plain rejected) for multi-user apps, automation platforms and\n    any client that should not hold\
  \ a long-lived secret. The same access token works on the Developer\n    API and on the MCP server.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth-v2.inflection.io/oauth2/authorize\n    tokenUrl: https://auth-v2.inflection.io/oauth2/token\n    revocationUrl: https://auth-v2.inflection.io/oauth2/revoke\n    introspectionUrl: https://auth-v2.inflection.io/oauth2/introspect\n    jwksUri: https://auth-v2.inflection.io/oauth2/jwks\n    registrationUrl: https://auth-v2.inflection.io/client-app/connect/register\n    scopes: [inflection_app]\n  discovery:\n    authorization_server_metadata: https://auth-v2.inflection.io/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://mcp.inflection.io/.well-known/oauth-protected-resource\n    specs: [RFC 8414, RFC 9728]\n  authorization_model: >-\n    Acts as the user who authorized the app — workspace admins and members read and write, viewers are\n    read-only. There is no client-credentials grant;\
  \ service-to-service tokens are rejected with 403.\n  token_lifetime_seconds: 900\n  refresh: refresh_token grant with rotation and reuse detection\n  authorization_code_ttl_seconds: 300\n  client_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt]\n  applies_to:\n  - https://api.inflection.io/v1\n  - https://mcp.inflection.io/\n  - https://campaign.inflection.io/api/v1\n  sources:\n  - https://docs.inflection.io/agents/connected-apps-oauth\n  - https://auth-v2.inflection.io/.well-known/oauth-authorization-server\n  see: scopes/inflectionio-scopes.yml\nfailures:\n  '401': >-\n    Missing, malformed, or invalid token. Also returned for unknown paths/methods under /v1\n    (deny-by-default) — a mistyped path is indistinguishable from a bad credential.\n  '403': >-\n    Token is valid but lacks the required permission — a READ-scoped PAT attempting a write, a viewer's\n    OAuth token doing the same, or a service-to-service token with no user behind it.\n  body: Gateway\
  \ auth errors (401/403) return an empty body; the status code carries the meaning.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/authentication/inflectionio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Saas
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- MCP
- Agents
- Artificial Intelligence
- Customer Journeys
- Webhook
---
