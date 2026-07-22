---
api_key_in: []
api_specs:
- filename: n3xt-openapi-original.json
  format: json
  label: N3XT API
  slug: n3xt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/openapi/n3xt-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: N3Xt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: N3XT secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: N3XT
provider_slug: n3xt
scheme_count: 2
schemes:
- description: Bearer auth -> insert ONLY the token (the word Bearer will automatically be added)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/n3xt-openapi-original.json
  type: http
- access_token_ttl_seconds: 3600
  flows:
  - docs: https://helpcenter.n3xt.io/en/articles/12118191-api-getting-started
    flow: clientCredentials
    tokenUrl: https://authn.n3xt.io/v1/oauth2/token
  - authorizationUrl: https://authn.n3xt.io
    flow: authorizationCode
    tokenUrl: https://authn.n3xt.io/v1/oauth2/token
  issuer: https://authn.n3xt.io
  name: OAuth2
  source: https://authn.n3xt.io/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: n3xt-authentication
source_filename: n3xt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/n3xt-openapi-original.json\ndocs: https://helpcenter.n3xt.io/en/articles/12118191-api-getting-started\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\nnotes: >-\n  The N3XT API operations declare a single `bearerAuth` (HTTP bearer / JWT)\n  security scheme. The bearer token is obtained out-of-band from the N3XT\n  authorization server at authn.n3xt.io using OAuth 2.0. Business API clients\n  use the client_credentials grant (client_id + client_secret issued under\n  Settings > API Keys); access tokens are bearer JWTs that expire after 3600s\n  (1 hour). The authorization server also publishes OpenID Connect discovery\n  and an authorization_code flow (used by first-party app sign-in and the MCP\n  server). Separate test authorization projects exist for the Beta and Omega\n  test environments.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme:\
  \ bearer\n  description: Bearer auth -> insert ONLY the token (the word Bearer will automatically be added)\n  sources:\n  - openapi/n3xt-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  source: https://authn.n3xt.io/.well-known/openid-configuration\n  issuer: https://authn.n3xt.io\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authn.n3xt.io/v1/oauth2/token\n    docs: https://helpcenter.n3xt.io/en/articles/12118191-api-getting-started\n  - flow: authorizationCode\n    authorizationUrl: https://authn.n3xt.io\n    tokenUrl: https://authn.n3xt.io/v1/oauth2/token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  access_token_ttl_seconds: 3600\nenvironments:\n  production:\n    token_url: https://authn.n3xt.io/v1/public/{project}/oauth2/token\n  beta:\n    token_url: https://authn.beta.n3xt.io/v1/public/{project}/oauth2/token\n  omega:\n    token_url: https://authn.omega.n3xt.io/v1/public/{project}/oauth2/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/authentication/n3xt-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Crypto
- Banking
- Payments
- Stablecoin
- Fintech
- Blockchain
- API
- MCP
---
