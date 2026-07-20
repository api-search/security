---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Dejbox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: Dejbox (Refectory) secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: Dejbox (Refectory)
provider_slug: dejbox
scheme_count: 2
schemes:
- issuer: https://customers.refectory.fr
  name: OpenIDConnect
  openIdConnectUrl: https://customers.refectory.fr/.well-known/openid-configuration
  sources:
  - well-known/dejbox-openid-configuration.json
  type: openIdConnect
- authorizationUrl: https://customers.refectory.fr/oauth2/auth
  endSessionUrl: https://customers.refectory.fr/oauth2/sessions/logout
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  id_token_signing_alg:
  - RS256
  jwksUri: https://customers.refectory.fr/.well-known/jwks.json
  name: OAuth2
  revocationUrl: https://customers.refectory.fr/oauth2/revoke
  sources:
  - well-known/dejbox-openid-configuration.json
  tokenUrl: https://customers.refectory.fr/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
  userinfoUrl: https://customers.refectory.fr/userinfo
slug: dejbox-authentication
source_filename: dejbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://customers.refectory.fr/.well-known/openid-configuration\ndocs: https://customers.refectory.fr/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://customers.refectory.fr/.well-known/openid-configuration\n  issuer: https://customers.refectory.fr\n  sources:\n  - well-known/dejbox-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  authorizationUrl: https://customers.refectory.fr/oauth2/auth\n  tokenUrl: https://customers.refectory.fr/oauth2/token\n  userinfoUrl: https://customers.refectory.fr/userinfo\n  revocationUrl: https://customers.refectory.fr/oauth2/revoke\n  endSessionUrl: https://customers.refectory.fr/oauth2/sessions/logout\n  jwksUri: https://customers.refectory.fr/.well-known/jwks.json\n\
  \  grant_types:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  id_token_signing_alg:\n  - RS256\n  sources:\n  - well-known/dejbox-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dejbox/refs/heads/main/authentication/dejbox-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Food & Agritech
- Corporate Catering
- Food Delivery
- B2B
- France
- Meal Delivery
- OAuth2
- OpenID Connect
---
