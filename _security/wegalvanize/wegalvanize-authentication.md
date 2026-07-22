---
api_key_in: []
api_specs:
- filename: wegalvanize-highbond-openapi-original.yml
  format: yaml
  label: HighBond API
  slug: highbond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/openapi/wegalvanize-highbond-openapi-original.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Wegalvanize Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- tokenExchange
- refreshToken
overview: Wegalvanize secures its APIs with http, oauth2, and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, tokenExchange, and refreshToken flow(s).
provider_name: Wegalvanize
provider_slug: wegalvanize
scheme_count: 1
schemes:
- applied: global
  bearerFormat: oauth2
  description: 'Industry-standard OAuth 2.0 bearer token for the HighBond platform, sent in the Authorization header. Declared as the single global security requirement across all operations.

    '
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/wegalvanize-highbond-openapi-original.yml
  type: http
slug: wegalvanize-authentication
source_filename: wegalvanize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wegalvanize-highbond-openapi-original.yml\ndocs: https://help.highbond.com/helpdocs/highbond/en-us/Default.htm#cshid=lp-access-tokens\noidc_discovery: https://oidc.highbond.com/.well-known/openid-configuration\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_scheme: bearer\n  bearer_format: oauth2\n  token_model: >\n    Personal / system-account API tokens minted in Launchpad and sent as\n    `Authorization: Bearer <TOKEN>`. Tokens are tied to a user (permissions\n    mirror that user's HighBond permissions; API access requires System Admin\n    on at least one instance) and, per the docs, are issued without an\n    expiration date. Underlying issuance uses the OAuth 2.0 Authorization Code\n    workflow.\n  oauth2_flows: [authorizationCode, clientCredentials, implicit, tokenExchange, refreshToken]\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: oauth2\n    applied: global\n\
  \    sources: [openapi/wegalvanize-highbond-openapi-original.yml]\n    description: >\n      Industry-standard OAuth 2.0 bearer token for the HighBond platform, sent\n      in the Authorization header. Declared as the single global security\n      requirement across all operations.\noidc:\n  issuer: https://oidc.highbond.com\n  authorization_endpoint: https://oidc.highbond.com/auth\n  token_endpoint: https://oidc.highbond.com/token\n  userinfo_endpoint: https://oidc.highbond.com/userinfo\n  jwks_uri: https://oidc.highbond.com/jwks\n  introspection_endpoint: https://oidc.highbond.com/tokeninfo\n  revocation_endpoint: https://oidc.highbond.com/token/revocation\n  end_session_endpoint: https://oidc.highbond.com/session/end\n  pushed_authorization_request_endpoint: https://oidc.highbond.com/request\n  grant_types_supported: [implicit, authorization_code, refresh_token, client_credentials, \"urn:ietf:params:oauth:grant-type:token-exchange\"]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported:\
  \ [client_secret_basic, client_secret_jwt, client_secret_post, private_key_jwt, none]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/authentication/wegalvanize-authentication.yml
summary_line: http/oauth2/openIdConnect · 1 scheme
tags:
- Company
- Governance
- Risk
- Compliance
- Audit
- GRC
- Analytics
- Automation
- Security
---
