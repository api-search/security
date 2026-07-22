---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Saib And Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SAIB & Co. secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SAIB & Co.
provider_slug: saib-and-co
scheme_count: 2
schemes:
- authorizationUrl: https://saibnco.cafe24api.com/api/v2/oauth/authorize
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: cafe24StorefrontOAuth
  revocationUrl: https://saibnco.cafe24api.com/api/v2/oauth/revoke
  sources:
  - well-known/saib-and-co-openid-configuration.json
  tokenUrl: https://saibnco.cafe24api.com/api/v2/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  type: oauth2
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - jti
  - at_hash
  - auth_time
  - nonce
  - amr
  - mall.name
  - mall.email
  - mall.gender
  - mall.birthdate
  - mall.phone_number
  - mall.address
  id_token_signing_alg_values:
  - RS256
  issuer: https://saibnco.cafe24api.com
  jwks_uri: https://saibnco.cafe24api.com/api/v2/.well-known/jwks.json
  name: cafe24OpenIDConnect
  openIdConnectUrl: https://saibnco.com/.well-known/openid-configuration
  sources:
  - well-known/saib-and-co-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://saibnco.cafe24api.com/api/v2/customers/userinfo
slug: saib-and-co-authentication
source_filename: saib-and-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://saibnco.com/.well-known/openid-configuration\ndocs: https://developers.cafe24.com/app/front/app/develop/oauth\nnotes: >-\n  Authentication is provided by the Cafe24 Unified Commerce Platform (UCP)\n  Storefront OAuth for the SAIB & Co. mall. Values below are taken verbatim\n  from the mall's live OpenID Connect discovery document; the issuer is the\n  mall-scoped Cafe24 API host saibnco.cafe24api.com.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  oidc_issuer: https://saibnco.cafe24api.com\nschemes:\n- name: cafe24StorefrontOAuth\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://saibnco.cafe24api.com/api/v2/oauth/authorize\n  tokenUrl: https://saibnco.cafe24api.com/api/v2/oauth/token\n  revocationUrl: https://saibnco.cafe24api.com/api/v2/oauth/revoke\n  token_endpoint_auth_methods: [client_secret_basic, none]\n  code_challenge_methods: [S256]\n\
  \  grant_types: [authorization_code, refresh_token]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- name: cafe24OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://saibnco.com/.well-known/openid-configuration\n  issuer: https://saibnco.cafe24api.com\n  userinfo_endpoint: https://saibnco.cafe24api.com/api/v2/customers/userinfo\n  jwks_uri: https://saibnco.cafe24api.com/api/v2/.well-known/jwks.json\n  id_token_signing_alg_values: [RS256]\n  claims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - jti\n  - at_hash\n  - auth_time\n  - nonce\n  - amr\n  - mall.name\n  - mall.email\n  - mall.gender\n  - mall.birthdate\n  - mall.phone_number\n  - mall.address\n  sources: [well-known/saib-and-co-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saib-and-co/refs/heads/main/authentication/saib-and-co-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Cosmetics
- Consumer Goods
- E-Commerce
- Wellness
- Retail
- Cafe24
- OAuth
---
