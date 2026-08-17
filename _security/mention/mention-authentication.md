---
api_key_in:
- query
api_specs:
- filename: mention-accounts-api-openapi.yml
  format: yaml
  label: Mention Accounts API
  slug: mention-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-accounts-api-openapi.yml
- filename: mention-alerts-api-openapi.yml
  format: yaml
  label: Mention Alerts API
  slug: mention-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-alerts-api-openapi.yml
- filename: mention-authors-api-openapi.yml
  format: yaml
  label: Mention Authors API
  slug: mention-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-authors-api-openapi.yml
- filename: mention-mentions-api-openapi.yml
  format: yaml
  label: Mention Mentions API
  slug: mention-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-mentions-api-openapi.yml
- filename: mention-shares-api-openapi.yml
  format: yaml
  label: Mention Shares API
  slug: mention-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-shares-api-openapi.yml
- filename: mention-stats-api-openapi.yml
  format: yaml
  label: Mention Stats API
  slug: mention-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-stats-api-openapi.yml
- filename: mention-tags-api-openapi.yml
  format: yaml
  label: Mention Tags API
  slug: mention-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tags-api-openapi.yml
- filename: mention-tasks-api-openapi.yml
  format: yaml
  label: Mention Tasks API
  slug: mention-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tasks-api-openapi.yml
- filename: mention-app-api-openapi.yml
  format: yaml
  label: Mention App API
  slug: mention-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-app-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mention Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mention secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mention
provider_slug: mention
scheme_count: 3
schemes:
- description: 'The documented and preferred transport: "This is the preferred way to pass tokens, as it doesn''t involve URL manipulations."'
  example_request: 'GET /api/accounts/me HTTP/1.1

    Host: api.mention.net

    Authorization: Bearer REDACTED_EXAMPLE_TOKEN

    '
  format: 'Authorization: Bearer <access_token>'
  location: Authorization header
  name: bearerAuth
  preferred: true
  scheme: bearer
  sources:
  - openapi/_original/mention-openapi.yml
  type: http
- description: The same token passed in the query string. Documented and supported, but discouraged by Mention itself — and it puts a full-authority credential into URLs, logs and referrers.
  example_request: GET /api/accounts/me?access_token=REDACTED_EXAMPLE_TOKEN
  in: query
  name: accessTokenQuery
  parameter: access_token
  preferred: false
  sources:
  - openapi/_original/mention-openapi.yml
  type: apiKey
- authorize_parameters:
  - name: client_id
    note: From the app's settings page.
  - name: redirect_uri
    note: Must be prefixed by one of the callback URLs registered on the app.
  - name: response_type
    note: code
  description: Authorization-code flow used to obtain an access token for a third party's Mention account. Skip it entirely if you only need your own account — use the token on your app's settings page.
  flows:
  - authorizationUrl: https://web.mention.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://web.mention.net/oauth/v2/token
  name: oauth2
  sources:
  - openapi/_original/mention-openapi.yml
  token_parameters:
  - name: client_id
  - name: client_secret
  - name: redirect_uri
    note: OAuth2 requires this to match the value used in the authorize step.
  - name: response_type
    note: Documented as "token" on the token exchange — a Mention-specific deviation; RFC 6749 defines no response_type on the token endpoint.
  - name: code
    note: The authorization code delivered to the callback in the query string.
  - name: grant_type
    note: authorization_code
  token_request:
    content_type: application/x-www-form-urlencoded
    method: POST
    note: GET is also accepted but explicitly discouraged. This is the only part of the API that is not JSON.
  token_response:
    expires_in: not returned
    refresh_token: not returned
    shape: '{"access_token": "...", "token_type": "bearer"}'
  type: oauth2
slug: mention-authentication
source_filename: mention-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://dev.mention.com/current/src/index.html (Authentication),\n  https://dev.mention.com/current/src/appendix/OAuth2.html,\n  https://dev.mention.com/current/src/guidelines/Clients.html, and the securitySchemes in\n  openapi/_original/mention-openapi.yml\ndocs: https://dev.mention.com/current/src/index.html\nsummary:\n  types:\n    - http\n    - apiKey\n    - oauth2\n  api_key_in:\n    - query\n  oauth2_flows:\n    - authorizationCode\n  scopes: 0\n  preferred: bearerAuth\n  note: >-\n    One credential, three ways to obtain or present it. Everything reduces to a bearer access token\n    that carries full authority over one account; there are no scopes and no least-privilege option.\n\nregistration:\n  required: true\n  step: Create an API client (an \"app\") before any call.\n  docs: https://dev.mention.com/current/src/guidelines/Clients.html\n  note: >-\n    \"Registering will give you an access token that will be\
  \ needed for your requests to the API.\"\n    The token for your own account is printed at the bottom of the app's settings page. The same\n    settings page holds the client_id and client_secret used by the OAuth2 flow, and the callback\n    URLs that redirect_uri must be prefixed by.\n  warning: >-\n    Mention states the personal access token \"gives full access to your account. Keep it\n    confidential.\" It is not scoped and no rotation or expiry policy is documented.\n\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    location: Authorization header\n    format: 'Authorization: Bearer <access_token>'\n    preferred: true\n    description: >-\n      The documented and preferred transport: \"This is the preferred way to pass tokens, as it\n      doesn't involve URL manipulations.\"\n    example_request: |\n      GET /api/accounts/me HTTP/1.1\n      Host: api.mention.net\n      Authorization: Bearer REDACTED_EXAMPLE_TOKEN\n    sources:\n      - openapi/_original/mention-openapi.yml\n\
  \  - name: accessTokenQuery\n    type: apiKey\n    in: query\n    parameter: access_token\n    preferred: false\n    description: >-\n      The same token passed in the query string. Documented and supported, but discouraged by Mention\n      itself — and it puts a full-authority credential into URLs, logs and referrers.\n    example_request: 'GET /api/accounts/me?access_token=REDACTED_EXAMPLE_TOKEN'\n    sources:\n      - openapi/_original/mention-openapi.yml\n  - name: oauth2\n    type: oauth2\n    description: >-\n      Authorization-code flow used to obtain an access token for a third party's Mention account.\n      Skip it entirely if you only need your own account — use the token on your app's settings page.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://web.mention.com/authorize\n        tokenUrl: https://web.mention.net/oauth/v2/token\n        scopes: 0\n    authorize_parameters:\n      - name: client_id\n        note: From the app's settings page.\n\
  \      - name: redirect_uri\n        note: Must be prefixed by one of the callback URLs registered on the app.\n      - name: response_type\n        note: code\n    token_parameters:\n      - name: client_id\n      - name: client_secret\n      - name: redirect_uri\n        note: OAuth2 requires this to match the value used in the authorize step.\n      - name: response_type\n        note: Documented as \"token\" on the token exchange — a Mention-specific deviation; RFC 6749 defines no response_type on the token endpoint.\n      - name: code\n        note: The authorization code delivered to the callback in the query string.\n      - name: grant_type\n        note: authorization_code\n    token_request:\n      method: POST\n      content_type: application/x-www-form-urlencoded\n      note: >-\n        GET is also accepted but explicitly discouraged. This is the only part of the API that is not\n        JSON.\n    token_response:\n      shape: '{\"access_token\": \"...\", \"token_type\"\
  : \"bearer\"}'\n      expires_in: not returned\n      refresh_token: not returned\n    sources:\n      - openapi/_original/mention-openapi.yml\n\ntoken_lifecycle:\n  expiry: not documented\n  refresh: not documented\n  revocation: not documented\n  rotation: not documented\n  introspection: not documented\n  note: >-\n    No expires_in, no refresh_token grant, no revocation endpoint and no introspection endpoint\n    appear anywhere in the reference. The only documented recovery from a rejected token is to\n    re-read it from the app settings page or re-run the authorization flow.\n\ndiscovery:\n  rfc8414_metadata: false\n  openid_configuration: false\n  note: >-\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration both return 404 on\n    mention.com and api.mention.com. The endpoints are discoverable only by reading the prose docs.\n\nfailure_modes:\n  - status: 401\n    body: '{\"error\":\"access_denied\",\"error_description\":\"OAuth2 authentication required\"\
  }'\n    observed:\n      url: https://api.mention.net/api/accounts/me\n      fetched: '2026-08-13'\n    meaning: No token, malformed token, or token no longer valid.\n  - status: 403\n    meaning: >-\n      Valid token, wrong subject. The reference repeats this rule for accounts and shares — a token\n      cannot act on another person's account even when the app created it, and deleting someone\n      else's share needs team-admin rights.\n  - status: 402\n    meaning: Valid token, but the account's plan does not cover the request or the parameter used.\n\nagent_notes:\n  - >-\n    A Mention token is all-or-nothing. There is no read-only credential, so an agent holding one can\n    delete accounts and delete shares — which destroys alerts and their collected mentions.\n  - >-\n    Constrain at the agent layer: see agentic-access/mention-agentic-access.yml for per-operation\n    action-class, consequence and human-in-the-loop contracts.\n  - Never use the access_token query parameter in\
  \ an agent; it leaks a full-authority credential into logs.\n\ncross_references:\n  scopes: scopes/mention-scopes.yml\n  conventions: conventions/mention-conventions.yml\n  errors: errors/mention-problem-types.yml\n  well_known: well-known/mention-well-known.yml\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/authentication/mention-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Alerts
- Brand Monitoring
- Media Monitoring
- Social Listening
- Social Media
- Sentiment Analysis
- Reputation Management
- Influencer Marketing
- Competitive Intelligence
- Streaming
- Marketing
---
