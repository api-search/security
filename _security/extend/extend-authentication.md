---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Extend Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Extend secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Extend
provider_slug: extend
scheme_count: 2
schemes:
- authorization_url: https://api.helloextend.com/auth/oauth/authorize
  description: An Admin or API Manager creates an API Integration in the Extend Merchant Portal, which issues an OAuth Client ID and Client Secret. These are exchanged for a short-lived access token via the token endpoint using grant_type=client_credentials.
  flow: clientCredentials
  grant_types:
  - client_credentials
  - iam_client_credentials
  id_token_signing_alg:
  - ES256
  - RS256
  introspection_url: https://api.helloextend.com/auth/oauth/introspect
  jwks_uri: https://api.helloextend.com/auth/oauth/keys
  name: OAuth2ClientCredentials
  token_url: https://api.helloextend.com/auth/oauth/token
  type: oauth2
- description: 'The access token obtained from the client-credentials exchange is passed on most requests in the X-Extend-Access-Token request header (not a standard Authorization: Bearer header).'
  in: header
  name: X-Extend-Access-Token
  type: apiKey
slug: extend-authentication
source_filename: extend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.extend.com/reference/authentication\ndocs: https://docs.extend.com/reference/authentication\ndiscovery: https://api.helloextend.com/.well-known/openid-configuration\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  access_token_header: X-Extend-Access-Token\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    An Admin or API Manager creates an API Integration in the Extend Merchant Portal, which\n    issues an OAuth Client ID and Client Secret. These are exchanged for a short-lived access\n    token via the token endpoint using grant_type=client_credentials.\n  token_url: https://api.helloextend.com/auth/oauth/token\n  authorization_url: https://api.helloextend.com/auth/oauth/authorize\n  introspection_url: https://api.helloextend.com/auth/oauth/introspect\n  jwks_uri: https://api.helloextend.com/auth/oauth/keys\n  id_token_signing_alg:\
  \ [ES256, RS256]\n  grant_types: [client_credentials, iam_client_credentials]\n- name: AccessTokenHeader\n  type: apiKey\n  in: header\n  name: X-Extend-Access-Token\n  description: >-\n    The access token obtained from the client-credentials exchange is passed on most requests in\n    the X-Extend-Access-Token request header (not a standard Authorization: Bearer header).\nenvironments:\n- name: production\n  base_url: https://api.helloextend.com\n- name: demo\n  base_url: https://api-demo.helloextend.com\n  note: Separate credentials must be created in the demo Merchant Portal (merchants.demo.extend.com).\nnotes: >-\n  Extend uses OAuth2 client-credentials to mint short-lived access tokens, then passes the token\n  in the custom X-Extend-Access-Token header rather than Authorization. No user-facing OAuth\n  scopes are documented (machine-to-machine client credentials), so no scopes/ artifact is\n  emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/authentication/extend-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Consumer
- Product Protection
- Extended Warranty
- Shipping Protection
- Ecommerce
- Warranty
- Claims
- Contracts
- Retail
- Insurance
---
