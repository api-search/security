---
api_key_in:
- query
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Adroll Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- refreshToken
overview: AdRoll secures its APIs with oauth2, apiKey, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and refreshToken flow(s).
provider_name: AdRoll
provider_slug: adroll
scheme_count: 5
schemes:
- description: The registered application's consumer key (client ID). Always sent in the URL query string regardless of HTTP method — the docs state explicitly that it must NOT be placed in the body of POST/PUT/PATCH requests.
  in: query
  name: apikey
  obtained_from: https://developers.nextroll.com/my-apps/new-app
  parameter: apikey
  required_on: every request to every service
  source: https://apidocs.nextroll.com/guides/api-key-migration.html
  type: apiKey
- description: Personal Access Token identifying the AdRoll user, for scripts and simple integrations. Created and revoked by the user at https://app.adroll.com/settings/personal-access-tokens. Must be paired with the application's client ID in the apikey query parameter.
  format: 'Authorization: Token MYTOKEN'
  header: Authorization
  in: header
  name: personalAccessToken
  scheme: Token
  source: https://apidocs.nextroll.com/guides/get-started.html
  type: http
- authorizationUrl: https://services.adroll.com/auth/authorize
  conforms_to:
  - RFC 6749
  - RFC 6750
  flows:
  - flow: authorizationCode
    note: three-legged; the most commonly used grant
  - flow: implicit
    note: for clients that cannot keep a secret, e.g. single-page apps
  - flow: password
    note: Resource Owner Password Credentials. The docs recommend it only when browser redirection is impossible.
  - flow: refreshToken
    note: Refresh tokens expire one year after issue AND on first use; a new refresh token is returned with every new access token.
  name: oauth2
  scopes:
  - all
  source: https://apidocs.nextroll.com/guides/oauth.html
  tokenUrl: https://services.adroll.com/auth/token
  token_lifetime:
    access_token: 24 hours (all grant types)
    refresh_token: 1 year, single-use
  token_transport:
  - 'Authorization: Bearer {ACCESS_TOKEN}'
  - form-encoded body parameter access_token={ACCESS_TOKEN}
  - URL query parameter ?access_token={ACCESS_TOKEN}
  type: oauth2
- applies_to: Server-to-Server (S2S) Event API — https://srv.adroll.com/api
  description: 'Server Access Tokens (SATs) are a separate credential class for the S2S event endpoint. They are not self-service: the docs say you must contact your account manager, and NextRoll shares the credential through a one-time 1Password share link that expires after seven days.'
  header: Authorization
  in: header
  name: serverAccessToken
  scheme: Token
  self_service: false
  source: https://apidocs.nextroll.com/server-to-server-api/reference.html
  type: http
- applies_to: AdRoll MCP Server — https://services.adroll.com/mcp
  authorizationUrl: https://services.adroll.com/mcp/auth/authorize
  code_challenge_methods:
  - S256
  conforms_to:
  - RFC 8414
  - RFC 9728
  - RFC 7591
  - PKCE RFC 7636
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  introspectionUrl: https://services.adroll.com/mcp/auth/introspect
  issuer: https://services.adroll.com/mcp
  name: mcpOAuth
  note: A separate authorization surface from the platform OAuth above, published as RFC 8414 / RFC 9728 metadata documents. This one supports Dynamic Client Registration and mandatory PKCE, which the platform OAuth guide does not mention.
  registrationUrl: https://services.adroll.com/mcp/auth/register
  revocationUrl: https://services.adroll.com/mcp/auth/revoke
  scopes:
  - mcp
  source: https://services.adroll.com/.well-known/oauth-authorization-server
  tokenUrl: https://services.adroll.com/mcp/auth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: adroll-authentication
source_filename: adroll-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://apidocs.nextroll.com/guides/get-started.html\ndocs: https://apidocs.nextroll.com/guides/oauth.html\nnote: >-\n  NextRoll publishes no OpenAPI file, so this profile is read from the published\n  auth guides rather than derived from securitySchemes. Every NextRoll API\n  requires TWO credentials at once: a user credential (OAuth access token or\n  Personal Access Token) in the Authorization header AND the registered\n  application's client ID in the `apikey` query parameter. Omitting the apikey\n  returns HTTP 401 apiproxy:3 even when the user credential is valid — verified\n  live against https://services.adroll.com/reporting/api/v1/query.\n\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode, implicit, password, refreshToken]\n  requires_two_credentials: true\n  registration_required: true\n  registration_url: https://developers.nextroll.com/accounts/create\n\nschemes:\n\
  - name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  required_on: every request to every service\n  description: >-\n    The registered application's consumer key (client ID). Always sent in the URL\n    query string regardless of HTTP method — the docs state explicitly that it\n    must NOT be placed in the body of POST/PUT/PATCH requests.\n  obtained_from: https://developers.nextroll.com/my-apps/new-app\n  source: https://apidocs.nextroll.com/guides/api-key-migration.html\n\n- name: personalAccessToken\n  type: http\n  scheme: Token\n  in: header\n  header: Authorization\n  format: 'Authorization: Token MYTOKEN'\n  description: >-\n    Personal Access Token identifying the AdRoll user, for scripts and simple\n    integrations. Created and revoked by the user at\n    https://app.adroll.com/settings/personal-access-tokens. Must be paired with\n    the application's client ID in the apikey query parameter.\n  source: https://apidocs.nextroll.com/guides/get-started.html\n\n\
  - name: oauth2\n  type: oauth2\n  conforms_to: [RFC 6749, RFC 6750]\n  authorizationUrl: https://services.adroll.com/auth/authorize\n  tokenUrl: https://services.adroll.com/auth/token\n  flows:\n  - flow: authorizationCode\n    note: three-legged; the most commonly used grant\n  - flow: implicit\n    note: for clients that cannot keep a secret, e.g. single-page apps\n  - flow: password\n    note: >-\n      Resource Owner Password Credentials. The docs recommend it only when\n      browser redirection is impossible.\n  - flow: refreshToken\n    note: >-\n      Refresh tokens expire one year after issue AND on first use; a new refresh\n      token is returned with every new access token.\n  token_lifetime:\n    access_token: 24 hours (all grant types)\n    refresh_token: 1 year, single-use\n  token_transport:\n  - 'Authorization: Bearer {ACCESS_TOKEN}'\n  - 'form-encoded body parameter access_token={ACCESS_TOKEN}'\n  - 'URL query parameter ?access_token={ACCESS_TOKEN}'\n  scopes: [all]\n\
  \  source: https://apidocs.nextroll.com/guides/oauth.html\n\n- name: serverAccessToken\n  type: http\n  scheme: Token\n  in: header\n  header: Authorization\n  applies_to: Server-to-Server (S2S) Event API — https://srv.adroll.com/api\n  description: >-\n    Server Access Tokens (SATs) are a separate credential class for the S2S event\n    endpoint. They are not self-service: the docs say you must contact your\n    account manager, and NextRoll shares the credential through a one-time\n    1Password share link that expires after seven days.\n  self_service: false\n  source: https://apidocs.nextroll.com/server-to-server-api/reference.html\n\n- name: mcpOAuth\n  type: oauth2\n  applies_to: AdRoll MCP Server — https://services.adroll.com/mcp\n  conforms_to: [RFC 8414, RFC 9728, RFC 7591, PKCE RFC 7636]\n  issuer: https://services.adroll.com/mcp\n  authorizationUrl: https://services.adroll.com/mcp/auth/authorize\n  tokenUrl: https://services.adroll.com/mcp/auth/token\n  registrationUrl: https://services.adroll.com/mcp/auth/register\n\
  \  revocationUrl: https://services.adroll.com/mcp/auth/revoke\n  introspectionUrl: https://services.adroll.com/mcp/auth/introspect\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  scopes: [mcp]\n  dynamic_client_registration: true\n  note: >-\n    A separate authorization surface from the platform OAuth above, published as\n    RFC 8414 / RFC 9728 metadata documents. This one supports Dynamic Client\n    Registration and mandatory PKCE, which the platform OAuth guide does not\n    mention.\n  source: https://services.adroll.com/.well-known/oauth-authorization-server\n\ntransport:\n  https_only: true\n  note: 'The docs state HTTPS is the only supported protocol.'\n\ngaps:\n- >-\n  Fine-grained OAuth scopes are not implemented — the docs say \"At this time, we\n  only support a single scope\" (`all`), with finer scopes \"in the future\". An\n  agent granted an AdRoll token\
  \ therefore holds full account access.\n- >-\n  Passing the access token in a URL query parameter is documented as a supported\n  option; tokens in URLs leak through logs, referrers and proxies.\n- >-\n  The S2S credential is distributed by human handoff (account manager + a\n  1Password share link), so it cannot be provisioned programmatically.\n\nx-evidence:\n  checked: '2026-08-13'\n  probes:\n  - {url: 'https://services.adroll.com/reporting/api/v1/query', http_status: 401, body: \"apiproxy:3 Missing 'apikey' query parameter\"}\n  - {url: 'https://services.adroll.com/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adroll/refs/heads/main/authentication/adroll-authentication.yml
summary_line: oauth2/apiKey/http · 5 schemes
tags:
- Advertising
- Display Advertising
- Retargeting
- Marketing
- AdTech
- Programmatic
---
