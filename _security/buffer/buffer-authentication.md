---
api_key_in:
- header
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Buffer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Buffer secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Buffer
provider_slug: buffer
scheme_count: 3
schemes:
- description: Personal API key. Acts on behalf of the issuing account only, and reaches every organization and channel that account can see — Buffer states plainly "There is no per-organization scoping at this time" and "The key is account-based, not organization-based". A request without a valid key returns 401 Unauthorized. This is the credential used by the CLI (BUFFER_API_KEY), by the generic MCP setup, and by the n8n, Cursor and Raycast integration guides.
  format: 'Authorization: Bearer <API_KEY>'
  in: header
  issued_at: https://publish.buffer.com/settings/api
  name: PersonalApiKey
  parameter: Authorization
  scheme: bearer
  scope_model: none
  source: https://developers.buffer.com/guides/authentication.html
  type: http
- access_token_lifetime_seconds: 3600
  authorization_url: https://auth.buffer.com/auth
  client_types:
  - credentials:
    - client_id
    - client_secret
    kind: confidential
    note: Sends client_secret AND code_verifier.
  - credentials:
    - client_id
    kind: public
    note: Mobile, desktop and single-page apps. Authenticate with the code_verifier alone and must NOT send a client_secret. The discovery document advertises token_endpoint_auth_methods_supported "none".
  code_challenge_methods:
  - S256
  description: Authorization Code flow with PKCE, required for all Buffer OAuth clients. Used by the Claude connector against the MCP server ("No API key needed").
  end_session_endpoint: https://auth.buffer.com/session/end
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  introspection_endpoint: https://auth.buffer.com/token/introspection
  issuer: https://auth.buffer.com
  jwks_uri: https://auth.buffer.com/jwks
  name: OAuth2AuthorizationCodePKCE
  pkce: required
  pushed_authorization_request_endpoint: https://auth.buffer.com/request
  refresh_tokens: rotating
  registration_endpoint: https://auth.buffer.com/reg
  source: https://developers.buffer.com/guides/authentication.html
  token_type: Bearer
  token_url: https://auth.buffer.com/token
  type: oauth2
  userinfo_endpoint: https://auth.buffer.com/me
- claims_supported:
  - sub
  - sid
  - auth_time
  - iss
  description: auth.buffer.com is a full OIDC provider. Note that Buffer's own authentication guide does not mention OIDC at all — this was found only by probing the discovery endpoint, which is why the artifact records it separately rather than folding it into the OAuth entry.
  id_token_signing_alg_values_supported:
  - PS256
  - RS256
  name: OpenIDConnect
  openIdConnectUrl: https://auth.buffer.com/.well-known/openid-configuration
  response_modes_supported:
  - form_post
  - fragment
  - query
  source: well-known/buffer-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
slug: buffer-authentication
source_filename: buffer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.buffer.com/guides/authentication.html\ndocs: https://developers.buffer.com/guides/authentication.html\nnote: >-\n  Derived-from-OpenAPI is not possible for Buffer — there is no OpenAPI. This\n  profile is read from Buffer's own authentication guide and corroborated\n  against the live OAuth/OIDC discovery documents saved in well-known/.\napi: Buffer GraphQL API\nendpoint: https://api.buffer.com\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  pkce_required: true\n  dynamic_client_registration: true\nschemes:\n  - name: PersonalApiKey\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Bearer <API_KEY>'\n    issued_at: https://publish.buffer.com/settings/api\n    scope_model: none\n    description: >-\n      Personal API key. Acts on behalf of the issuing account\
  \ only, and reaches\n      every organization and channel that account can see — Buffer states\n      plainly \"There is no per-organization scoping at this time\" and \"The key\n      is account-based, not organization-based\". A request without a valid key\n      returns 401 Unauthorized. This is the credential used by the CLI\n      (BUFFER_API_KEY), by the generic MCP setup, and by the n8n, Cursor and\n      Raycast integration guides.\n    source: https://developers.buffer.com/guides/authentication.html\n  - name: OAuth2AuthorizationCodePKCE\n    type: oauth2\n    flow: authorizationCode\n    pkce: required\n    code_challenge_methods: [S256]\n    authorization_url: https://auth.buffer.com/auth\n    token_url: https://auth.buffer.com/token\n    registration_endpoint: https://auth.buffer.com/reg\n    pushed_authorization_request_endpoint: https://auth.buffer.com/request\n    introspection_endpoint: https://auth.buffer.com/token/introspection\n    userinfo_endpoint: https://auth.buffer.com/me\n\
  \    end_session_endpoint: https://auth.buffer.com/session/end\n    jwks_uri: https://auth.buffer.com/jwks\n    issuer: https://auth.buffer.com\n    grant_types: [authorization_code, refresh_token, client_credentials]\n    token_type: Bearer\n    access_token_lifetime_seconds: 3600\n    refresh_tokens: rotating\n    client_types:\n      - kind: confidential\n        credentials: [client_id, client_secret]\n        note: Sends client_secret AND code_verifier.\n      - kind: public\n        credentials: [client_id]\n        note: >-\n          Mobile, desktop and single-page apps. Authenticate with the\n          code_verifier alone and must NOT send a client_secret. The discovery\n          document advertises token_endpoint_auth_methods_supported \"none\".\n    description: >-\n      Authorization Code flow with PKCE, required for all Buffer OAuth clients.\n      Used by the Claude connector against the MCP server (\"No API key needed\").\n    source: https://developers.buffer.com/guides/authentication.html\n\
  \  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://auth.buffer.com/.well-known/openid-configuration\n    id_token_signing_alg_values_supported: [PS256, RS256]\n    claims_supported: [sub, sid, auth_time, iss]\n    subject_types_supported: [public]\n    response_modes_supported: [form_post, fragment, query]\n    description: >-\n      auth.buffer.com is a full OIDC provider. Note that Buffer's own\n      authentication guide does not mention OIDC at all — this was found only\n      by probing the discovery endpoint, which is why the artifact records it\n      separately rather than folding it into the OAuth entry.\n    source: well-known/buffer-openid-configuration.json\ntoken_rotation:\n  refresh_token_single_use: true\n  detail: >-\n    Buffer's guide carries an explicit warning: \"Refresh tokens are single-use.\n    Every successful refresh returns a new refresh_token and invalidates the\n    one you sent... Reusing an old refresh token revokes all tokens\
  \ for that\n    grant\" — the user must then re-authorize. Agents holding Buffer tokens must\n    persist the newest refresh token atomically.\nrevocation:\n  user_initiated: true\n  detail: >-\n    Users can revoke an app from Buffer account settings at any time; all\n    tokens for that app are invalidated and the API returns 401 Unauthorized.\n  connected_apps_query: Account.connectedApps in the GraphQL schema surfaces the granted clients.\nerrors:\n  authorization_redirect:\n    - {error: access_denied, meaning: The user denied your app.}\n    - {error: invalid_request, meaning: The request is missing or has invalid parameters.}\n    - {error: invalid_client, meaning: The client_id is not recognized.}\n    - {error: invalid_grant, meaning: The code is expired, already used, or invalid.}\n    - {error: invalid_scope, meaning: The requested scope is not valid.}\n  token_exchange_shape: '{\"error\": \"invalid_grant\", \"error_description\": \"Authorization code has expired\"}'\n  api_unauthenticated:\
  \ '{\"errors\":[{\"message\":\"An authentication JWT or Access Token is required\",\"extensions\":{\"code\":\"UNAUTHENTICATED\"}}]}'\nsecurity_guidance_published:\n  - Never commit the API key to version control.\n  - Do not expose it in client-side code; call from a server.\n  - Store it in an environment variable such as BUFFER_API_KEY.\n  - Rotate the key from Settings -> API if compromised.\nscopes: scopes/buffer-scopes.yml\nx-evidence:\n  - {fetched: '2026-08-13', url: 'https://developers.buffer.com/guides/authentication.html', http_status: 200}\n  - {fetched: '2026-08-13', url: 'https://auth.buffer.com/.well-known/openid-configuration', http_status: 200}\n  - {fetched: '2026-08-13', url: 'https://auth.buffer.com/.well-known/oauth-authorization-server', http_status: 200}\n  - {fetched: '2026-08-13', url: 'https://api.buffer.com', http_status: 401, note: anonymous GraphQL POST returns UNAUTHENTICATED}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buffer/refs/heads/main/authentication/buffer-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Social-Media
- Scheduling
- Analytics
- Publishing
- Content Management
- Social Media Management
- Social Media Marketing
- Marketing
- Content Scheduling
- GraphQL
- MCP
- Agents
---
