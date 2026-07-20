---
api_key_in: []
api_specs:
- filename: corti-transcribe-asyncapi.json
  format: json
  label: Corti Speech to Text API
  slug: corti-speech-to-text-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-transcribe-asyncapi.json
- filename: corti-stream-asyncapi.json
  format: json
  label: Corti Ambient Documentation API
  slug: corti-ambient-documentation-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-stream-asyncapi.json
auth_types:
- oauth2
- openIdConnect
description: 'Corti uses OAuth 2.0 client credentials (Keycloak / OpenID Connect) for server-to-server access to the Corti API. Clients exchange a client_id and client_secret at the realm token endpoint for a short-lived (5 minute) bearer access token, then call the API with an Authorization: Bearer header plus a required Tenant-Name header identifying the tenant context (default "base"). Limited-scope tokens (scope "openid transcribe" / "openid streams") can be minted for browser-side real-time streaming. The Embedded Assistant uses a separate token flow. Corti recommends client credentials over static API keys for short blast radius, scope granularity, and enterprise IdP/tenancy integration.'
kind: authentication
layout: security
method: searched
name: Corti Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Corti secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Corti
provider_slug: corti
scheme_count: 2
schemes:
- description: OAuth 2.0 client credentials via Corti Auth (Keycloak realm)
  flows:
  - flow: clientCredentials
    scopes_count: 57
    tokenUrl: https://auth.eu.corti.app/realms/{tenant}/protocol/openid-connect/token
  name: CortiAuth
  sources:
  - docs
  - well-known/corti-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  type: oauth2
- bearerFormat: JWT
  description: Short-lived JWT access token presented on each API request
  name: BearerAuth
  scheme: bearer
  sources:
  - docs
  type: http
slug: corti-authentication
source_filename: corti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.corti.ai/authentication/overview\ndocs: https://docs.corti.ai/authentication/overview\ndescription: >-\n  Corti uses OAuth 2.0 client credentials (Keycloak / OpenID Connect) for\n  server-to-server access to the Corti API. Clients exchange a client_id and\n  client_secret at the realm token endpoint for a short-lived (5 minute) bearer\n  access token, then call the API with an Authorization: Bearer header plus a\n  required Tenant-Name header identifying the tenant context (default \"base\").\n  Limited-scope tokens (scope \"openid transcribe\" / \"openid streams\") can be\n  minted for browser-side real-time streaming. The Embedded Assistant uses a\n  separate token flow. Corti recommends client credentials over static API keys\n  for short blast radius, scope granularity, and enterprise IdP/tenancy integration.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [clientCredentials, authorizationCode]\n\
  \  token_ttl_seconds: 300\n  required_headers: [Authorization, Tenant-Name]\n  identity_provider: Keycloak (OpenID Connect)\nschemes:\n- name: CortiAuth\n  type: oauth2\n  description: OAuth 2.0 client credentials via Corti Auth (Keycloak realm)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.eu.corti.app/realms/{tenant}/protocol/openid-connect/token\n    scopes_count: 57\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, tls_client_auth]\n  sources: [docs, well-known/corti-openid-configuration.json]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived JWT access token presented on each API request\n  sources: [docs]\nenvironments:\n- name: eu\n  auth_server: https://auth.eu.corti.app\n  api_base: https://api.eu.corti.app/v2\n- name: us\n  auth_server: https://auth.us.corti.app\n  api_base: https://api.us.corti.app/v2\n- name: beta-eu\n  auth_server: https://auth.beta-eu.corti.app\n\
  \  api_base: https://api.beta-eu.corti.app/v2\nnotes:\n- The Embedded Assistant authenticates differently; see https://docs.corti.ai/assistant/authentication\n- Agents (A2A) MCP calls support authorizationType none/inherit; inherit reuses the caller bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/authentication/corti-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Health
- Healthcare
- Artificial Intelligence
- Speech to Text
- Medical Coding
- Clinical Documentation
- Agents
- Machine Learning
---
