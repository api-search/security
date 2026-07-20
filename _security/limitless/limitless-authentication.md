---
api_key_in:
- header
api_specs:
- filename: limitless-developer-openapi-original.yml
  format: yaml
  label: Limitless Developer API
  slug: developer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limitless/refs/heads/main/openapi/limitless-developer-openapi-original.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Limitless Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Limitless secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Limitless
provider_slug: limitless
scheme_count: 3
schemes:
- description: Primary authentication for the REST API. Every request must carry the API key in the X-API-Key header. Keys are created in Developer settings in the Limitless Desktop or Web app (https://app.limitless.ai).
  in: header
  name: X-API-Key
  parameter_name: X-API-Key
  source: https://www.limitless.ai/developers
  spec_declared: false
  type: apiKey
- authorizationUrl: https://api.limitless.ai/api/auth/authorize
  description: OAuth 2.0 authorization server fronting the hosted MCP server at https://api.limitless.ai/mcp. Supports dynamic client registration (RFC 7591) and advertises itself as an MCP OAuth authorization server (MCP protocol 2025-06-18).
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: LimitlessOAuth
  pkce: S256
  registrationUrl: https://api.limitless.ai/api/auth/register
  revocationUrl: https://api.limitless.ai/api/auth/revoke
  scopes:
  - openid
  - profile
  - email
  - lifelogs:read
  source: well-known/limitless-oauth-authorization-server.json
  tokenUrl: https://api.limitless.ai/api/auth/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
- claims_supported:
  - sub
  - name
  - email
  - email_verified
  - preferred_username
  - updated_at
  end_session_endpoint: https://api.limitless.ai/api/auth/signout
  id_token_signing_alg_values_supported:
  - HS256
  issuer: https://api.limitless.ai
  name: LimitlessOIDC
  openIdConnectUrl: https://api.limitless.ai/.well-known/openid-configuration
  source: well-known/limitless-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://api.limitless.ai/api/auth/session
slug: limitless-authentication
source_filename: limitless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/limitless-developer-openapi-original.yml\ndocs: https://www.limitless.ai/developers\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    The published Swagger 2.0 document declares NO securityDefinitions, so no auth\n    profile could be derived mechanically from the spec. This profile was captured\n    from the developer documentation and from the live /.well-known/ discovery\n    documents on api.limitless.ai.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  description: >-\n    Primary authentication for the REST API. Every request must carry the API key in\n    the X-API-Key header. Keys are created in Developer settings in the Limitless\n    Desktop or Web app (https://app.limitless.ai).\n  source: https://www.limitless.ai/developers\n  spec_declared: false\n- name: LimitlessOAuth\n\
  \  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.limitless.ai/api/auth/authorize\n  tokenUrl: https://api.limitless.ai/api/auth/token\n  revocationUrl: https://api.limitless.ai/api/auth/revoke\n  registrationUrl: https://api.limitless.ai/api/auth/register\n  pkce: S256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  grant_types:\n  - authorization_code\n  - refresh_token\n  scopes:\n  - openid\n  - profile\n  - email\n  - lifelogs:read\n  description: >-\n    OAuth 2.0 authorization server fronting the hosted MCP server at\n    https://api.limitless.ai/mcp. Supports dynamic client registration (RFC 7591) and\n    advertises itself as an MCP OAuth authorization server (MCP protocol 2025-06-18).\n  source: well-known/limitless-oauth-authorization-server.json\n- name: LimitlessOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://api.limitless.ai/.well-known/openid-configuration\n  issuer: https://api.limitless.ai\n  userinfo_endpoint: https://api.limitless.ai/api/auth/session\n\
  \  end_session_endpoint: https://api.limitless.ai/api/auth/signout\n  id_token_signing_alg_values_supported:\n  - HS256\n  claims_supported:\n  - sub\n  - name\n  - email\n  - email_verified\n  - preferred_username\n  - updated_at\n  source: well-known/limitless-openid-configuration.json\nkey_management:\n  create: https://app.limitless.ai\n  path: Developer settings -> Create API Key\n  rotation_policy: not published\nrelated:\n  scopes: scopes/limitless-scopes.yml\n  conventions: conventions/limitless-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limitless/refs/heads/main/authentication/limitless-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Artificial Intelligence
- Wearables
- Voice
- Transcription
- Personal Data
- Consumer Hardware
- Search
- Productivity
- Meeting Notes
- Model Context Protocol
---
