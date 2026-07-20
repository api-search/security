---
api_key_in: []
auth_types:
- oauth2
description: 'The 180 Seguros Sagas API is protected with OAuth2 using the client-credentials (machine-to-machine) grant, brokered by an Auth0 tenant. Clients exchange a client_id + client_secret for a bearer access token (default lifetime 43,200s / 12 hours) and send it on every request as `Authorization: Bearer {access_token}`. The docs advise reusing tokens while valid rather than minting a new one per call.'
kind: authentication
layout: security
method: searched
name: 180 Insurance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: 180 Insurance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: 180 Insurance
provider_slug: 180-insurance
scheme_count: 1
schemes:
- bearer_header: 'Authorization: Bearer {access_token}'
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  sources:
  - docs.180s.com.br/reference/autenticacao
  - well-known/180-insurance-oauth-authorization-server.json
  token_lifetime_seconds: 43200
  token_url: https://180s-staging.us.auth0.com/oauth/token
  type: oauth2
slug: 180-insurance-authentication
source_filename: 180-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.180s.com.br/reference/autenticacao\ndocs: https://docs.180s.com.br/reference/autenticacao\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt]\n  identity_provider: Auth0\ndescription: >-\n  The 180 Seguros Sagas API is protected with OAuth2 using the client-credentials\n  (machine-to-machine) grant, brokered by an Auth0 tenant. Clients exchange a\n  client_id + client_secret for a bearer access token (default lifetime 43,200s /\n  12 hours) and send it on every request as `Authorization: Bearer {access_token}`.\n  The docs advise reusing tokens while valid rather than minting a new one per call.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://180s-staging.us.auth0.com/oauth/token\n  grant_type: client_credentials\n  token_lifetime_seconds: 43200\n  bearer_header:\
  \ 'Authorization: Bearer {access_token}'\n  sources: [docs.180s.com.br/reference/autenticacao, well-known/180-insurance-oauth-authorization-server.json]\nnotes: >-\n  No granular API scope surface is documented — access is scoped per M2M client /\n  distribution channel at grant time rather than via request scopes, so no\n  scopes/ artifact is emitted. The Auth0 tenant advertises the standard OIDC\n  scopes only (openid/profile/email/...), which apply to interactive flows, not\n  the API's client-credentials grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/authentication/180-insurance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Brazil
- Fintech
- API
- Webhooks
---
