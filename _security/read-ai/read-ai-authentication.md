---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: 'Read AI''s REST API and MCP server share one OAuth 2.1 authorization server (authn.read.ai) and one bearer-token contract. There are no static API keys: the provider explicitly documents this as a known limitation of the open beta, with personal access tokens planned for GA. Client credentials are obtained by RFC 7591 dynamic client registration; the user then completes a browser authorization-code flow with PKCE. Access tokens live 10 minutes and refresh tokens rotate on every use.'
kind: authentication
layout: security
method: searched
name: Read Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- clientCredentials
- deviceCode
- implicit
overview: Read AI secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, clientCredentials, deviceCode, and implicit flow(s).
provider_name: Read AI
provider_slug: read-ai
scheme_count: 2
schemes:
- audience:
  - https://api.read.ai/v1/meetings
  - https://api.read.ai/mcp
  flows:
  - authorizationUrl: https://authn.read.ai/oauth2/auth
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    pkce: true
    refreshUrl: https://authn.read.ai/oauth2/token
    tokenUrl: https://authn.read.ai/oauth2/token
  - deviceAuthorizationUrl: https://authn.read.ai/oauth2/device/auth
    flow: deviceCode
  - flow: clientCredentials
    note: Advertised in authorization-server metadata as a supported grant type; the provider's own docs say machine-to-machine use is not yet supported in the open beta.
    tokenUrl: https://authn.read.ai/oauth2/token
  id_token_signing_alg:
  - RS256
  issuer: https://authn.read.ai/
  jwks_uri: https://authn.read.ai/.well-known/jwks.json
  name: OAuth2
  registration_endpoint: https://api.read.ai/oauth/register
  revocation_endpoint: https://authn.read.ai/oauth2/revoke
  sources:
  - well-known/read-ai-openid-configuration.json
  - well-known/read-ai-oauth-authorization-server.json
  - well-known/read-ai-oauth-protected-resource-mcp.json
  spec: OAuth 2.1
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
  userinfo_endpoint: https://authn.read.ai/userinfo
- bearerFormat: JWT
  description: 'Every REST endpoint requires "Authorization: Bearer <access_token>". Tokens are Ory-issued (ory_at_... prefix) JWTs from the authorization-code exchange.'
  in: header
  name: BearerToken
  parameter: Authorization
  scheme: bearer
  sources:
  - https://support.read.ai/hc/en-us/articles/49381161088659-API-Reference
  type: http
slug: read-ai-authentication
source_filename: read-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication\ndocs: https://support.read.ai/hc/en-us/articles/49380809380371-API-Keys-Authentication\ndescription: >-\n  Read AI's REST API and MCP server share one OAuth 2.1 authorization server\n  (authn.read.ai) and one bearer-token contract. There are no static API keys: the\n  provider explicitly documents this as a known limitation of the open beta, with\n  personal access tokens planned for GA. Client credentials are obtained by RFC 7591\n  dynamic client registration; the user then completes a browser authorization-code\n  flow with PKCE. Access tokens live 10 minutes and refresh tokens rotate on every\n  use.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, clientCredentials, deviceCode, implicit]\n  static_api_keys: false\n  dynamic_client_registration: true\nschemes:\n  - name: OAuth2\n\
  \    type: oauth2\n    spec: OAuth 2.1\n    issuer: https://authn.read.ai/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://authn.read.ai/oauth2/auth\n        tokenUrl: https://authn.read.ai/oauth2/token\n        refreshUrl: https://authn.read.ai/oauth2/token\n        pkce: true\n        code_challenge_methods: [S256, plain]\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://authn.read.ai/oauth2/device/auth\n      - flow: clientCredentials\n        tokenUrl: https://authn.read.ai/oauth2/token\n        note: >-\n          Advertised in authorization-server metadata as a supported grant type; the\n          provider's own docs say machine-to-machine use is not yet supported in the\n          open beta.\n    registration_endpoint: https://api.read.ai/oauth/register\n    revocation_endpoint: https://authn.read.ai/oauth2/revoke\n    userinfo_endpoint: https://authn.read.ai/userinfo\n    jwks_uri: https://authn.read.ai/.well-known/jwks.json\n  \
  \  token_endpoint_auth_methods:\n      [client_secret_post, client_secret_basic, private_key_jwt, none]\n    id_token_signing_alg: [RS256]\n    audience:\n      - https://api.read.ai/v1/meetings\n      - https://api.read.ai/mcp\n    sources:\n      - well-known/read-ai-openid-configuration.json\n      - well-known/read-ai-oauth-authorization-server.json\n      - well-known/read-ai-oauth-protected-resource-mcp.json\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    parameter: Authorization\n    description: >-\n      Every REST endpoint requires \"Authorization: Bearer <access_token>\". Tokens are\n      Ory-issued (ory_at_... prefix) JWTs from the authorization-code exchange.\n    sources:\n      - https://support.read.ai/hc/en-us/articles/49381161088659-API-Reference\ntoken_lifetimes:\n  access_token_seconds: 600\n  refresh_token_rotation: true\n  refresh_token_single_use: true\n  refresh_grace_period: >-\n    Short, undocumented grace\
  \ window to tolerate concurrency; the previous refresh\n    token must be discarded after each exchange.\nend_user_authentication:\n  sso: [Microsoft, Google, SAML]\n  saml_providers_documented: [Okta, Microsoft Entra, Duo]\n  scim: true\n  scim_note: SAML & SCIM are Enterprise+ plan features.\n  mfa: true\nprerequisites:\n  - >-\n    If the caller belongs to a workspace, that workspace must have the Downloads\n    option enabled under Workspace Settings > Reports & Sharing.\n  - >-\n    A caller can only retrieve reports they can already see in the web app; admins\n    must enable Global Report Access to reach every report in a workspace.\nknown_limitations:\n  - No static API keys or personal access tokens (planned for GA).\n  - Browser-based login required; not yet suited to unattended machine-to-machine use.\n  - >-\n    Some MCP clients (VS Code, Notion have been reported) do not complete the\n    provider's auth flow.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n    - {url:\
  \ 'https://api.read.ai/v1/meetings', http_status: 401}\n    - {url: 'https://authn.read.ai/.well-known/openid-configuration', http_status: 200}\n    - {url: 'https://api.read.ai/.well-known/oauth-protected-resource/mcp', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/read-ai/refs/heads/main/authentication/read-ai-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Meeting Intelligence
- Artificial Intelligence
- Transcription
- Productivity
- Collaboration
- Model Context Protocol
- Agents
- Webhooks
- SaaS
---
