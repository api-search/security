---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tellius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tellius declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Tellius
provider_slug: tellius
scheme_count: 4
schemes:
- applies_to: Insights APIs, Search APIs, and the wider backend REST surface
  bearerFormat: JWT
  expiry: Documented only as a "temporary access token". No lifetime, no refresh operation is published for this scheme.
  id: telliusJwt
  issuance:
    content_type: application/json
    operation: POST https://{tellius-deployment-host}/api/auth/login
    request: '{"username": "...", "password": "..."}'
    required_headers:
    - name: csrf
      note: 'Docs: "Make sure the csrf header is passed (usually found in the page source when you are logged into Tellius)." No programmatic way to obtain the CSRF value is documented, which is the single largest friction point for a headless integrator on this surface.'
    response: '{"id": "<uuid>", "message": "Login successful", "token": "<jwt>"}'
  scheme: bearer
  type: http
  usage: 'Authorization: Bearer <token> on each call. The Insights API examples show the token sent as a bare Authorization value without the Bearer prefix; the docs are inconsistent here.'
- applies_to: browser-based applications
  id: telliusSession
  issuance: 'POST /api/auth/login with "session": true in the body.'
  note: Tellius creates a server-side session and manages authentication via cookies; no Authorization header is then needed. Recommended by the docs for browser apps.
  type: cookie
- applies_to: ML Model APIs (/proxy/ml/external/*)
  content_type: application/x-www-form-urlencoded
  flow: clientCredentials
  id: telliusOAuthClientCredentials
  parameters:
  - client_id
  - client_secret
  - grant_type (must be client_credentials)
  refresh:
    endpoint: POST https://{tellius-deployment-host}/oauth/refresh_token
    parameters:
    - refresh_token
    - secret
    - grant_type (must be refresh_token)
  response: '{"access_token": "...", "refresh_token": "...", "token_type": "bearer"}'
  scopes: []
  scopes_note: No scope parameter is documented for this flow.
  token_endpoint: POST https://{tellius-deployment-host}/oauth/client_credentials_token
  type: oauth2
- applies_to: the Tellius MCP server at /mcp
  authorization_endpoint: https://{tellius-deployment-host}/oauth/authorize
  discovery:
    authorization_server_metadata: /.well-known/oauth-authorization-server
    protected_resource_metadata: /.well-known/oauth-protected-resource
    standards:
    - RFC 8414
    - RFC 9728
    - RFC 7591
    - RFC 7636
  dynamic_client_registration: true
  flows:
  - authorizationCode
  - clientCredentials
  id: telliusMcpOAuth
  method: probed
  note: This is the strongest auth surface Tellius ships and the only one that is fully machine-discoverable. Browser sign-in needs no administrator; client id/secret credentials are created by an administrator under Admin Settings for headless clients.
  pkce: S256
  probe:
    date: '2026-08-30'
    http_status: 401
    url: https://qa1.dev.tellius.com/mcp
    www_authenticate: Bearer resource_metadata="https://qa1.dev.tellius.com/.well-known/oauth-protected-resource"
  registration_endpoint: https://{tellius-deployment-host}/oauth/register
  scopes:
  - mcp
  token_endpoint: https://{tellius-deployment-host}/oauth/token
  type: oauth2
slug: tellius-authentication
source_filename: tellius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://help.tellius.com/api/authentication-api-login-api\ndocs:\n- https://help.tellius.com/api/authentication-api-login-api\n- https://help.tellius.com/api/ml-model-apis\n- https://help.tellius.com/kaiya/tellius-mcp-server\n- https://help.tellius.com/settings/security/authentication\n- https://help.tellius.com/settings/security/sso-configuration\nname: Tellius authentication profile\nnote: 'Derived from Tellius'' published API and security documentation plus a live\n  probe of a Tellius deployment''s OAuth metadata. There is no OpenAPI definition, so\n  no securitySchemes block exists to derive from; derive-authentication.py had no\n  spec to read.'\n\nschemes:\n- id: telliusJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: Insights APIs, Search APIs, and the wider backend REST surface\n  issuance:\n    operation: 'POST https://{tellius-deployment-host}/api/auth/login'\n    content_type: application/json\n\
  \    request: '{\"username\": \"...\", \"password\": \"...\"}'\n    response: '{\"id\": \"<uuid>\", \"message\": \"Login successful\", \"token\": \"<jwt>\"}'\n    required_headers:\n    - name: csrf\n      note: 'Docs: \"Make sure the csrf header is passed (usually found in the page\n        source when you are logged into Tellius).\" No programmatic way to obtain the\n        CSRF value is documented, which is the single largest friction point for a\n        headless integrator on this surface.'\n  usage: 'Authorization: Bearer <token> on each call. The Insights API examples show\n    the token sent as a bare Authorization value without the Bearer prefix; the docs\n    are inconsistent here.'\n  expiry: 'Documented only as a \"temporary access token\". No lifetime, no refresh\n    operation is published for this scheme.'\n- id: telliusSession\n  type: cookie\n  applies_to: browser-based applications\n  issuance: 'POST /api/auth/login with \"session\": true in the body.'\n  note: 'Tellius\
  \ creates a server-side session and manages authentication via cookies;\n    no Authorization header is then needed. Recommended by the docs for browser apps.'\n- id: telliusOAuthClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  applies_to: ML Model APIs (/proxy/ml/external/*)\n  token_endpoint: 'POST https://{tellius-deployment-host}/oauth/client_credentials_token'\n  content_type: application/x-www-form-urlencoded\n  parameters:\n  - client_id\n  - client_secret\n  - grant_type (must be client_credentials)\n  response: '{\"access_token\": \"...\", \"refresh_token\": \"...\", \"token_type\": \"bearer\"}'\n  refresh:\n    endpoint: 'POST https://{tellius-deployment-host}/oauth/refresh_token'\n    parameters:\n    - refresh_token\n    - secret\n    - grant_type (must be refresh_token)\n  scopes: []\n  scopes_note: 'No scope parameter is documented for this flow.'\n- id: telliusMcpOAuth\n  type: oauth2\n  flows:\n  - authorizationCode\n  - clientCredentials\n  applies_to: the\
  \ Tellius MCP server at /mcp\n  pkce: S256\n  scopes:\n  - mcp\n  authorization_endpoint: https://{tellius-deployment-host}/oauth/authorize\n  token_endpoint: https://{tellius-deployment-host}/oauth/token\n  registration_endpoint: https://{tellius-deployment-host}/oauth/register\n  dynamic_client_registration: true\n  discovery:\n    authorization_server_metadata: /.well-known/oauth-authorization-server\n    protected_resource_metadata: /.well-known/oauth-protected-resource\n    standards:\n    - RFC 8414\n    - RFC 9728\n    - RFC 7591\n    - RFC 7636\n  method: probed\n  probe:\n    url: https://qa1.dev.tellius.com/mcp\n    http_status: 401\n    www_authenticate: 'Bearer resource_metadata=\"https://qa1.dev.tellius.com/.well-known/oauth-protected-resource\"'\n    date: '2026-08-30'\n  note: 'This is the strongest auth surface Tellius ships and the only one that is\n    fully machine-discoverable. Browser sign-in needs no administrator; client\n    id/secret credentials are created by\
  \ an administrator under Admin Settings for\n    headless clients.'\n\nend_user_authentication:\n  note: 'Platform sign-in, distinct from API credentials. Configured under Settings →\n    Security.'\n  methods:\n  - Default (local Tellius accounts)\n  - LDAP\n  - SAML 2.0 (Okta, Azure AD, OneLogin named in the docs, with auto-provisioning)\n  - OIDC (Okta, Google, Azure AD named)\n  - Azure AD\n  docs: https://help.tellius.com/settings/security/sso-configuration\n\nembedded_authentication:\n  note: 'Embedded Vizpads, Insights, Search, Assistant, Kaiya and Feeds authenticate\n    through the embedding URL plus postMessage, with row-level policy filters applied\n    per userId token.'\n  docs: https://help.tellius.com/embedding-tellius/embedding-url\n\nauthorization:\n  model: 'User-scoped. Every API and MCP request runs as a specific Tellius user;\n    Business View permissions, security tags, groups and row-level security policies\n    determine what that user can read.'\n  docs: https://help.tellius.com/settings/users-and-access/security-tags\n\
  \ngaps:\n- 'No public token-lifetime, rotation or revocation policy for the JWT login scheme.'\n- 'The csrf header requirement on /api/auth/login is documented as something you find\n  in page source, with no headless path stated.'\n- 'A single \"mcp\" scope covers every MCP tool including the destructive ones.'\n- 'No API-key scheme is offered for server-to-server REST use outside the ML endpoints.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tellius/refs/heads/main/authentication/tellius-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Analytics
- Business Intelligence
- Agentic Analytics
- Decision Intelligence
- Artificial Intelligence
- Machine-Learning
- Data
- Embedded Analytics
- MCP
- Natural Language Query
- Pharmaceuticals
- Consumer Packaged Goods
- Financial Planning
---
