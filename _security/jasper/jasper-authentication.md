---
api_key_in:
- header
api_specs:
- filename: jasper-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-attachments-api-openapi.yml
- filename: jasper-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-audiences-api-openapi.yml
- filename: jasper-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-command-api-openapi.yml
- filename: jasper-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-documents-api-openapi.yml
- filename: jasper-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-image-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-image-templates-api-openapi.yml
- filename: jasper-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-images-api-openapi.yml
- filename: jasper-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-knowledge-api-openapi.yml
- filename: jasper-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-projects-api-openapi.yml
- filename: jasper-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-styles-api-openapi.yml
- filename: jasper-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-tasks-api-openapi.yml
- filename: jasper-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-templates-api-openapi.yml
- filename: jasper-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-usage-api-openapi.yml
- filename: jasper-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-users-api-openapi.yml
- filename: jasper-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-voices-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Jasper Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Jasper secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Jasper
provider_slug: jasper
scheme_count: 3
schemes:
- description: Workspace-scoped API token sent in the X-API-KEY request header. Token management is restricted to users with the Admin or Developer role and is done at https://app.jasper.ai/settings/dev-tools/tokens. API access requires the Jasper Business plan.
  in: header
  name: ApiKeyAuth
  parameter_name: X-API-KEY
  type: apiKey
- description: 'OAuth 2.0 authorization-code flow with PKCE (S256) and Dynamic Client Registration, used by the hosted MCP server and agent integrations. Bearer access token sent as Authorization: Bearer.'
  flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://api.jasper.ai/oauth2/introspect
    issuer: https://api.jasper.ai
    pkce: S256
    registrationUrl: https://api.jasper.ai/oauth2/register
    revocationUrl: https://api.jasper.ai/oauth2/revoke
    scopes:
    - mcp
    - user:read
    - user
    - openid
    - email
    - profile
    tokenUrl: https://api.jasper.ai/oauth2/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: OAuth2
  type: oauth2
- description: OIDC discovery is published; response_types [code], scopes include openid/email/profile.
  name: OpenIDConnect
  openIdConnectUrl: https://api.jasper.ai/.well-known/openid-configuration
  type: openIdConnect
slug: jasper-authentication
source_filename: jasper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.jasper.ai/docs/authentication ;\n  https://api.jasper.ai/.well-known/openid-configuration ;\n  https://api.jasper.ai/.well-known/oauth-authorization-server ;\n  https://mcp.jasper.ai/.well-known/oauth-protected-resource ;\n  openapi/jasper-api-openapi.yml\ndocs: https://developers.jasper.ai/docs/authentication\nspec_confirmation: >-\n  Confirmed against the OpenAPI captured this round: components.securitySchemes declares `X-API-Key`\n  (apiKey, in header, name X-API-Key) and `oauth2` (authorizationCode flow, authorize/token/refresh\n  at https://api.jasper.ai/oauth2/*). There is no global `security` object — all 50 operations\n  declare `security: [{X-API-Key: []}, {oauth2: [user]}]` individually, so both schemes are\n  accepted everywhere and neither is optional.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n\
  \  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    Workspace-scoped API token sent in the X-API-KEY request header. Token management is\n    restricted to users with the Admin or Developer role and is done at\n    https://app.jasper.ai/settings/dev-tools/tokens. API access requires the Jasper Business plan.\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code flow with PKCE (S256) and Dynamic Client Registration, used by\n    the hosted MCP server and agent integrations. Bearer access token sent as Authorization: Bearer.\n  flows:\n  - flow: authorizationCode\n    issuer: https://api.jasper.ai\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\n    revocationUrl: https://api.jasper.ai/oauth2/revoke\n    introspectionUrl: https://api.jasper.ai/oauth2/introspect\n    registrationUrl: https://api.jasper.ai/oauth2/register\n    pkce: S256\n    grant_types: [authorization_code,\
  \ refresh_token]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    scopes: [mcp, user:read, user, openid, email, profile]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.jasper.ai/.well-known/openid-configuration\n  description: OIDC discovery is published; response_types [code], scopes include openid/email/profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/authentication/jasper-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
---
