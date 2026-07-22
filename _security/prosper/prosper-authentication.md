---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Prosper Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
- authorizationCode
overview: Prosper secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, refresh_token, and authorizationCode flow(s).
provider_name: Prosper
provider_slug: prosper
scheme_count: 3
schemes:
- description: Individual and institutional investors obtain an access token by posting their OAuth client credentials together with their Prosper account username/password to the token endpoint.
  flow: password
  grant_type: password
  name: OAuth2Password
  parameters:
  - grant_type
  - client_id
  - client_secret
  - username
  - password
  sources:
  - https://developers.prosper.com/docs/investor/
  token_url: https://api.prosper.com/v1/security/oauth/token
  type: oauth2
- description: Exchange a refresh_token for a new access token when it expires.
  flow: refresh_token
  grant_type: refresh_token
  name: OAuth2Refresh
  parameters:
  - grant_type
  - client_id
  - client_secret
  - refresh_token
  sources:
  - https://developers.prosper.com/docs/investor/
  token_url: https://api.prosper.com/v1/security/oauth/token
  type: oauth2
- authorization_url: https://www.prosper.com/oauth
  description: Third-party agents that trade on an investor's behalf request access through the Prosper consent screen; the investor grants permission per company.
  flow: authorizationCode
  grant_type: authorization_code
  name: OAuth2AuthorizationCode
  sources:
  - https://developers.prosper.com/docs/investor/
  - https://www.prosper.com/blog/prosper-announces-new-api-platform-for-investors
  token_url: https://api.prosper.com/v1/security/oauth/token
  type: oauth2
slug: prosper-authentication
source_filename: prosper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.prosper.com/docs/investor/\ndocs: https://developers.prosper.com/docs/investor/\nsummary:\n  types:\n  - oauth2\n  transport: SSL/TLS required (HTTPS only)\n  oauth2_flows:\n  - password\n  - refresh_token\n  - authorizationCode\nnotes: >-\n  Prosper does not publish an OpenAPI document; this profile is derived from the\n  provider's public developer documentation. The Investor API authenticates with\n  OAuth 2.0 over SSL. Prosper assigns each application a client_id and\n  client_secret on the OAuth Settings page. Named OAuth scopes are not\n  documented (there is no per-scope permission surface); third-party access is\n  authorized per-investor via the consent screen at https://www.prosper.com/oauth.\nschemes:\n- name: OAuth2Password\n  type: oauth2\n  flow: password\n  token_url: https://api.prosper.com/v1/security/oauth/token\n  grant_type: password\n  parameters:\n  - grant_type\n  - client_id\n  - client_secret\n\
  \  - username\n  - password\n  description: >-\n    Individual and institutional investors obtain an access token by posting\n    their OAuth client credentials together with their Prosper account\n    username/password to the token endpoint.\n  sources:\n  - https://developers.prosper.com/docs/investor/\n- name: OAuth2Refresh\n  type: oauth2\n  flow: refresh_token\n  token_url: https://api.prosper.com/v1/security/oauth/token\n  grant_type: refresh_token\n  parameters:\n  - grant_type\n  - client_id\n  - client_secret\n  - refresh_token\n  description: Exchange a refresh_token for a new access token when it expires.\n  sources:\n  - https://developers.prosper.com/docs/investor/\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://www.prosper.com/oauth\n  token_url: https://api.prosper.com/v1/security/oauth/token\n  grant_type: authorization_code\n  description: >-\n    Third-party agents that trade on an investor's behalf request access\
  \ through\n    the Prosper consent screen; the investor grants permission per company.\n  sources:\n  - https://developers.prosper.com/docs/investor/\n  - https://www.prosper.com/blog/prosper-announces-new-api-platform-for-investors\nrequest_header: 'Authorization: bearer <access_token>'\nenvironments:\n  production:\n    base_url: https://api.prosper.com/v1\n    token_url: https://api.prosper.com/v1/security/oauth/token\n  sandbox:\n    base_url: https://api.sandbox.prosper.com/v1\n    token_url: https://api.sandbox.prosper.com/v1/security/oauth/token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosper/refs/heads/main/authentication/prosper-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Company
- Fintech
- Lending
- Peer-to-Peer Lending
- Marketplace Lending
- Investing
- Personal Loans
- Consumer Credit
- Financial Services
---
