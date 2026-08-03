---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Knowde Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- refreshToken
overview: Knowde secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and refreshToken flow(s).
provider_name: Knowde
provider_slug: knowde
scheme_count: 2
schemes:
- access_token_lifetime_seconds: 86400
  client_authentication: HTTP Basic (Base64 client_id:client_secret) or form parameters
  flow: clientCredentials
  grant_type: client_credentials
  issues_refresh_token: true
  media_type: application/x-www-form-urlencoded
  name: OAuth2ClientCredentials
  scopes: []
  sources:
  - https://developer.knowde.com/documentation/auth
  tokenUrl: https://developer-api.knowde.com/oauth/token
  type: oauth2
- flow: refreshToken
  grant_type: refresh_token
  media_type: application/x-www-form-urlencoded
  name: OAuth2RefreshToken
  sources:
  - https://developer.knowde.com/documentation/auth
  tokenUrl: https://developer-api.knowde.com/oauth/token
  type: oauth2
slug: knowde-authentication
source_filename: knowde-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://developer.knowde.com/documentation/auth\ndocs: https://developer.knowde.com/documentation/auth\nnotes: 'Derived from the public Knowde API Authorization documentation. Knowde publishes\n  no OpenAPI or GraphQL SDL on a public URL (the REST and GraphQL references at\n  developer.knowde.com/documentation/rest and /documentation/graphql redirect to\n  https://www.knowde.com/sign-in), so this profile is transcribed from the docs\n  rather than derived from securitySchemes.'\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - refreshToken\n  api_key_in: []\n  token_type: Bearer\n  auth_host: https://developer-api.knowde.com\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://developer-api.knowde.com/oauth/token\n  media_type: application/x-www-form-urlencoded\n  client_authentication: HTTP Basic (Base64 client_id:client_secret) or form parameters\n\
  \  grant_type: client_credentials\n  access_token_lifetime_seconds: 86400\n  issues_refresh_token: true\n  scopes: []\n  sources:\n  - https://developer.knowde.com/documentation/auth\n- name: OAuth2RefreshToken\n  type: oauth2\n  flow: refreshToken\n  tokenUrl: https://developer-api.knowde.com/oauth/token\n  grant_type: refresh_token\n  media_type: application/x-www-form-urlencoded\n  sources:\n  - https://developer.knowde.com/documentation/auth\ntoken_usage:\n  header: 'Authorization: Bearer {access_token}'\n  uri_query_parameter_supported: false\n  uri_query_parameter_note: 'Knowde explicitly does not support sending access tokens\n    as URI parameters (RFC 6750 section 2.3).'\nrevocation:\n  supported: true\n  endpoint: https://developer-api.knowde.com/oauth/revoke\n  standard: RFC 7009 OAuth 2.0 Token Revocation\n  client_authentication: 'Authorization: Basic Base64(client_id:client_secret)'\n  behavior: Always returns 200 OK, even when the token does not exist or is already\n   \
  \ revoked. A client may only revoke tokens it was issued.\n  sources:\n  - https://developer.knowde.com/documentation/auth\ncredentials:\n  provisioning: API Clients are created and deleted in the Knowde Developer Portal.\n  requires: Company admin role, and the Knowde API must be enabled for the company\n    (arranged through a Knowde sales representative).\n  secret_display: Client id and client secret are displayed only once at creation.\n  docs: https://developer.knowde.com/documentation/api_clients\nscope_surface:\n  published: false\n  note: Knowde documents no OAuth scope or permission reference on its public developer\n    site; access appears to be bound to the API Client and the company's subscription\n    rather than to per-request scopes. No scopes/ artifact is emitted rather than\n    inventing one.\nguidance:\n  token_reuse: Knowde advises requesting tokens sparingly, keeping the number of active\n    tokens to a minimum, and not requesting a token per work item; excessive\
  \ token\n    requests may be rate limited.\nx-evidence:\n- fetched: '2026-08-01'\n  url: https://developer.knowde.com/documentation/auth\n  http_status: 200\n- fetched: '2026-08-01'\n  url: https://developer-api.knowde.com/graphql\n  http_status: 401\n  note: POST of a GraphQL introspection query returns {\"message\":\"Unauthorized\"},\n    confirming the GraphQL endpoint exists and is authentication-gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowde/refs/heads/main/authentication/knowde-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Chemicals
- Ingredients
- Marketplace
- Master Data Management
- Product Information Management
- Manufacturing
- Distribution
- B2B Commerce
- GraphQL
- Artificial Intelligence
---
