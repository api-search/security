---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aircover-openapi.yml
  format: yaml
  label: Aircover Public Agent API
  slug: aircover-public-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/openapi/aircover-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aircover Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aircover secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aircover
provider_slug: aircover
scheme_count: 1
schemes:
- challenge: 'Unauthenticated POST https://api.aircover.ai/mcp returned 401 with WWW-Authenticate: Bearer resource_metadata="https://api.aircover.ai/.well-known/oauth-protected-resource" (observed 2026-09-19 via the x-amzn-remapped-www-authenticate header on the API Gateway edge).'
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration (RFC 7591). Agents register a client at /oauth/register (redirect_uris required — a live POST with an empty body returned 400 invalid_client_metadata "redirect_uris is required"), send the user to /oauth/authorize, exchange the code at /oauth/token, and refresh without human intervention beyond the initial consent. A token's scope caps what the client may request and every request is additionally bounded by the authorizing user's own role and organization. Tokens are revocable at /oauth/revoke.
  flows:
  - authorizationUrl: https://api.aircover.ai/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.aircover.ai/oauth/token
    scopes: 1
    tokenUrl: https://api.aircover.ai/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: oauth2
  registration_endpoint: https://api.aircover.ai/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.aircover.ai/oauth/revoke
  scopes_supported:
  - mcp
  sources:
  - openapi/aircover-openapi.yml
  - https://api.aircover.ai/.well-known/oauth-authorization-server
  - https://www.aircover.ai/developers
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: aircover-authentication
source_filename: aircover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.aircover.ai/developers\nderived_from: openapi/aircover-openapi.yml\ndocs: https://www.aircover.ai/developers\ndiscovery:\n  oauth_authorization_server: https://api.aircover.ai/.well-known/oauth-authorization-server\n  oauth_protected_resource: https://api.aircover.ai/.well-known/oauth-protected-resource\n  saved:\n  - well-known/aircover-oauth-authorization-server.json\n  - well-known/aircover-oauth-protected-resource.json\n  probed: '2026-09-19'\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  dynamic_client_registration: true\n  pkce: S256\n  api_keys: false\n  note: >-\n    The only public credential is an OAuth 2.0 bearer token minted by Aircover's own authorization server\n    (issuer https://api.aircover.ai). There is no API-key scheme on the public agent surface. The customer\n    REST API used by the aircover-pipeline CLI authenticates separately with username/password at\n    POST\
  \ /auth/login or a bearer token copied from the web app; that surface is customer-only and undocumented\n    publicly.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.aircover.ai/oauth/authorize\n    tokenUrl: https://api.aircover.ai/oauth/token\n    refreshUrl: https://api.aircover.ai/oauth/token\n    scopes: 1\n  registration_endpoint: https://api.aircover.ai/oauth/register\n  revocation_endpoint: https://api.aircover.ai/oauth/revoke\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  scopes_supported:\n  - mcp\n  description: >-\n    OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration (RFC 7591). Agents\n    register a client at /oauth/register (redirect_uris required — a live POST with an empty\
  \ body returned\n    400 invalid_client_metadata \"redirect_uris is required\"), send the user to /oauth/authorize, exchange the\n    code at /oauth/token, and refresh without human intervention beyond the initial consent. A token's scope\n    caps what the client may request and every request is additionally bounded by the authorizing user's own\n    role and organization. Tokens are revocable at /oauth/revoke.\n  challenge: >-\n    Unauthenticated POST https://api.aircover.ai/mcp returned 401 with\n    WWW-Authenticate: Bearer resource_metadata=\"https://api.aircover.ai/.well-known/oauth-protected-resource\"\n    (observed 2026-09-19 via the x-amzn-remapped-www-authenticate header on the API Gateway edge).\n  sources:\n  - openapi/aircover-openapi.yml\n  - https://api.aircover.ai/.well-known/oauth-authorization-server\n  - https://www.aircover.ai/developers\nend_user_sign_in:\n  note: >-\n    End users of the Aircover app sign in with Google OAuth, Microsoft OAuth (Azure AD) or a per-organization\n\
  \    OIDC/SSO provider (Okta, Auth0, Azure AD B2C). Personal email domains are refused; new sign-ups receive\n    a trial license. These are the identities an MCP client's OAuth consent screen delegates to; they are not\n    themselves API credentials.\n  methods:\n  - Google OAuth (requests calendar scopes; Drive scopes optional for CMS indexing)\n  - Microsoft OAuth / Azure AD (requests Microsoft Graph calendar scopes; OneDrive optional)\n  - OIDC / SSO configured per customer organization\n  source: https://www.aircover.ai/llms.txt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircover/refs/heads/main/authentication/aircover-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Sales Enablement
- Conversation Intelligence
- Sales Coaching
- Revenue Intelligence
- AI Agents
- MCP
- agent-native
- CRM
- Meetings
- Transcription
- Authentication
---
