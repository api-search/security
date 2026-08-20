---
api_key_in: []
api_specs:
- filename: canva-assets-api-openapi.yml
  format: yaml
  label: Canva Assets API
  slug: canva-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-assets-api-openapi.yml
- filename: canva-autofills-api-openapi.yml
  format: yaml
  label: Canva Autofills API
  slug: canva-autofills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-autofills-api-openapi.yml
- filename: canva-brand-templates-api-openapi.yml
  format: yaml
  label: Canva Brand Templates API
  slug: canva-brand-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-brand-templates-api-openapi.yml
- filename: canva-comments-api-openapi.yml
  format: yaml
  label: Canva Comments API
  slug: canva-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-comments-api-openapi.yml
- filename: canva-designs-api-openapi.yml
  format: yaml
  label: Canva Designs API
  slug: canva-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-designs-api-openapi.yml
- filename: canva-exports-api-openapi.yml
  format: yaml
  label: Canva Exports API
  slug: canva-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-exports-api-openapi.yml
- filename: canva-folders-api-openapi.yml
  format: yaml
  label: Canva Folders API
  slug: canva-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-folders-api-openapi.yml
- filename: canva-resizes-api-openapi.yml
  format: yaml
  label: Canva Resizes API
  slug: canva-resizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-resizes-api-openapi.yml
- filename: canva-users-api-openapi.yml
  format: yaml
  label: Canva Users API
  slug: canva-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-users-api-openapi.yml
- filename: canva-connect-api-openapi.yml
  format: yaml
  label: Canva Connect API
  slug: canva-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/openapi/canva-connect-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Canva Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Canva secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Canva
provider_slug: canva
scheme_count: 2
schemes:
- description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included in the Authorization header as a Bearer token.
  flows:
  - authorizationUrl: https://www.canva.com/api/oauth/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://api.canva.com/rest/v1/oauth/token
  name: oauth2
  sources:
  - openapi/canva-assets-api-openapi.yml
  - openapi/canva-autofills-api-openapi.yml
  - openapi/canva-brand-templates-api-openapi.yml
  - openapi/canva-comments-api-openapi.yml
  - openapi/canva-connect-api-openapi.yml
  - openapi/canva-designs-api-openapi.yml
  - openapi/canva-exports-api-openapi.yml
  - openapi/canva-folders-api-openapi.yml
  - openapi/canva-resizes-api-openapi.yml
  - openapi/canva-users-api-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/canva-connect-api-openapi.yml
  type: http
slug: canva-authentication
source_filename: canva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.canva.dev/docs/connect/authentication/ + https://www.canva.com/.well-known/openid-configuration\n  + https://www.canva.com/.well-known/oauth-authorization-server + openapi/canva-connect-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.canva.com/api/oauth/authorize\n    tokenUrl: https://api.canva.com/rest/v1/oauth/token\n    scopes: 11\n  description: Canva uses OAuth 2.0 with authorization code flow. Access tokens must be included in the\n    Authorization header as a Bearer token.\n  sources:\n  - openapi/canva-assets-api-openapi.yml\n  - openapi/canva-autofills-api-openapi.yml\n  - openapi/canva-brand-templates-api-openapi.yml\n  - openapi/canva-comments-api-openapi.yml\n  - openapi/canva-connect-api-openapi.yml\n  - openapi/canva-designs-api-openapi.yml\n\
  \  - openapi/canva-exports-api-openapi.yml\n  - openapi/canva-folders-api-openapi.yml\n  - openapi/canva-resizes-api-openapi.yml\n  - openapi/canva-users-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/canva-connect-api-openapi.yml\ndocs: https://www.canva.dev/docs/connect/authentication/\ndiscovery:\n  oauth_authorization_server:\n    url: https://www.canva.com/.well-known/oauth-authorization-server\n    status: 200\n    file: well-known/canva-oauth-authorization-server.json\n  openid_configuration:\n    url: https://www.canva.com/.well-known/openid-configuration\n    status: 200\n    file: well-known/canva-openid-configuration.json\n  issuer: https://www.canva.com\n  authorization_endpoint: https://www.canva.com/api/oauth/authorize\n  token_endpoint: https://api.canva.com/auth/v1/oauth/token\n  userinfo_endpoint: https://api.canva.com/auth/v1/oidc/userinfo\n  jwks_uri: https://api.canva.com/auth/v1/oidc/jwks\n  note: Canva runs the OAuth/OIDC\
  \ endpoints on auth/v1 (api.canva.com/auth/v1/oauth/token) per its discovery\n    documents, while the Connect OpenAPI documents the equivalent token endpoint under the REST path /rest/v1/oauth/token.\n    Both are Canva-published; prefer the discovery document.\npkce:\n  required: true\n  methods:\n  - S256\n  source: https://www.canva.dev/docs/connect/api-requests-responses/\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\ngrant_types:\n- authorization_code\n- refresh_token\ntoken_lifecycle:\n  introspection: POST /v1/oauth/introspect (introspectToken)\n  revocation: POST /v1/oauth/revoke (revokeTokens) — revokes a token and its lineage\n  refresh: refresh_token grant\nbasic_auth_note: The basicAuth securityScheme in the OpenAPI is CLIENT authentication on the OAuth token\n  endpoints (client_id/client_secret), not a way to call resource endpoints. Every resource operation\n  requires a bearer token from the authorization code flow.\nmcp:\n  endpoint: https://mcp.canva.com/mcp\n\
  \  auth: oauth\n  dynamic_client_registration: true\n  detail: mcp/canva-mcp.yml\nscopes: scopes/canva-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/authentication/canva-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Application
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
---
