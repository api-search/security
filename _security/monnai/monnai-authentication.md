---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Monnai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Monnai secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Monnai
provider_slug: monnai
scheme_count: 1
schemes:
- description: Monnai secures its Insights API with OAuth 2.0. Access tokens are issued by Monnai's hosted authorization server (AWS-fronted, awselb/2.0 behind CloudFront). Machine-to-machine integrations obtain a bearer token from the token endpoint and present it on each API call; the console uses the authorization-code flow for interactive sign-in.
  environments:
    development:
      authorization: https://auth-dev.monnai.com/oauth2/authorize
      logout: https://auth-dev.monnai.com/logout
      token: https://auth-dev.monnai.com/oauth2/token
    production:
      authorization: https://auth.monnai.com/oauth2/authorize
      token: https://auth.monnai.com/oauth2/token
  flows:
  - authorizationUrl: https://auth.monnai.com/oauth2/authorize
    flow: authorizationCode
    logoutUrl: https://auth.monnai.com/logout
    tokenUrl: https://auth.monnai.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.monnai.com/oauth2/token
  name: MonnaiOAuth2
  type: oauth2
slug: monnai-authentication
source_filename: monnai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  Live probes of Monnai OAuth2 authorization server (auth.monnai.com,\n  auth-dev.monnai.com) + endpoint constants harvested from the Monnai developer\n  console application (dev.monnai.com/bundle.js).\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\nschemes:\n  - name: MonnaiOAuth2\n    type: oauth2\n    description: >-\n      Monnai secures its Insights API with OAuth 2.0. Access tokens are issued by\n      Monnai's hosted authorization server (AWS-fronted, awselb/2.0 behind\n      CloudFront). Machine-to-machine integrations obtain a bearer token from the\n      token endpoint and present it on each API call; the console uses the\n      authorization-code flow for interactive sign-in.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.monnai.com/oauth2/authorize\n        tokenUrl: https://auth.monnai.com/oauth2/token\n        logoutUrl:\
  \ https://auth.monnai.com/logout\n      - flow: clientCredentials\n        tokenUrl: https://auth.monnai.com/oauth2/token\n    environments:\n      production:\n        authorization: https://auth.monnai.com/oauth2/authorize\n        token: https://auth.monnai.com/oauth2/token\n      development:\n        authorization: https://auth-dev.monnai.com/oauth2/authorize\n        token: https://auth-dev.monnai.com/oauth2/token\n        logout: https://auth-dev.monnai.com/logout\nevidence:\n  - host: auth.monnai.com\n    observed: >-\n      GET / -> 200 (awselb/2.0 via CloudFront); POST /oauth2/token -> 405 on empty\n      body (real token endpoint, method/param-gated).\n  - host: auth-dev.monnai.com\n    observed: OAuth2 authorize/token/logout endpoints referenced by the developer console bundle.\nnotes: >-\n  No public /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n  document is exposed (both return 404 JSON from the authorization server). Scope\n  reference is\
  \ not published on a public page, so no scopes/ artifact was derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monnai/refs/heads/main/authentication/monnai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer Insights
- Fintech
- Financial Services
- Fraud Detection
- Identity Verification
- KYC
- AML
- Credit Decisioning
- Risk Assessment
- Collections
- Emerging Markets
- Decisioning
- OAuth2
---
