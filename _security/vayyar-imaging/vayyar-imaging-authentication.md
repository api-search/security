---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: 'Vayyar publishes no OpenAPI, so no securitySchemes could be derived. The only documented authentication surface found is on the Walabot DIY storefront (walabot.com, Shopify): customer-account OAuth 2.0 / OIDC published via RFC 8414 discovery at /.well-known/oauth-authorization-server and OIDC discovery at /.well-known/openid-configuration (both saved verbatim under well-known/). Authorization code flow with PKCE (S256), RS256 ID tokens, issuer https://shopify.com/authentication/10514071618, endpoints hosted on account.walabot.com. The storefront''s UCP MCP endpoint additionally requires a UCP agent-profile handshake, and read-only storefront browsing (/products/{handle}.json) requires no authentication. The Walabot SDK (api.walabot.com) is a local USB device library with no network authentication.'
kind: authentication
layout: security
method: searched
name: Vayyar Imaging Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vayyar Imaging secures its APIs with oauth2, openIdConnect, and none across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vayyar Imaging
provider_slug: vayyar-imaging
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://account.walabot.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.walabot.com/authentication/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/10514071618
  name: walabot-customer-account-oidc
  openIdConnectUrl: https://walabot.com/.well-known/openid-configuration
  sources:
  - well-known/vayyar-imaging-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
slug: vayyar-imaging-authentication
source_filename: vayyar-imaging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://walabot.com/.well-known/openid-configuration\ndocs: https://walabot.com/llms.txt\ndescription: >-\n  Vayyar publishes no OpenAPI, so no securitySchemes could be derived. The only\n  documented authentication surface found is on the Walabot DIY storefront\n  (walabot.com, Shopify): customer-account OAuth 2.0 / OIDC published via RFC\n  8414 discovery at /.well-known/oauth-authorization-server and OIDC discovery\n  at /.well-known/openid-configuration (both saved verbatim under well-known/).\n  Authorization code flow with PKCE (S256), RS256 ID tokens, issuer\n  https://shopify.com/authentication/10514071618, endpoints hosted on\n  account.walabot.com. The storefront's UCP MCP endpoint additionally requires\n  a UCP agent-profile handshake, and read-only storefront browsing\n  (/products/{handle}.json) requires no authentication. The Walabot SDK\n  (api.walabot.com) is a local USB device library with no network\n  authentication.\n\
  summary:\n  types: [oauth2, openIdConnect, none]\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  notes: read-only storefront JSON endpoints are unauthenticated\nschemes:\n  - name: walabot-customer-account-oidc\n    type: openIdConnect\n    openIdConnectUrl: https://walabot.com/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/10514071618\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.walabot.com/authentication/oauth/authorize\n        tokenUrl: https://account.walabot.com/authentication/oauth/token\n    grant_types: [authorization_code, refresh_token, \"urn:ietf:params:oauth:grant-type:jwt-bearer\"]\n    token_endpoint_auth_methods: [client_secret_basic]\n    code_challenge_methods: [S256]\n    id_token_signing_alg: [RS256]\n    sources: [well-known/vayyar-imaging-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayyar-imaging/refs/heads/main/authentication/vayyar-imaging-authentication.yml
summary_line: oauth2/openIdConnect/none · 1 scheme
tags:
- Company
- Sensors
- Radar
- Imaging
- IoT
- Healthcare
- Elderly Care
- Automotive
- Smart Home
---
