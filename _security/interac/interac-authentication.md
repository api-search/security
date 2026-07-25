---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Interac Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- refreshToken
overview: Interac secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, and refreshToken flow(s).
provider_name: Interac
provider_slug: interac
scheme_count: 2
schemes:
- issuer: https://gateway-portal.hub-verify.innovation.interac.ca/
  name: openid_connect
  openIdConnectUrl: https://gateway-portal.hub-verify.innovation.interac.ca/.well-known/openid-configuration
  sources:
  - well-known/interac-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth
    flow: authorizationCode
    pushedAuthorizationRequestUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth/par
    refreshUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token
    tokenUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token
  grant_types_supported:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  name: oauth2
  type: oauth2
slug: interac-authentication
source_filename: interac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://gateway-portal.hub-verify.innovation.interac.ca/.well-known/openid-configuration\ndocs: https://documents.hub-verify.innovation.interac.ca/docs/quick-start-guide\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, refreshToken]\n  oidc: true\n  par_required: true\n  request_object: true          # signed JWT request parameter (JAR)\n  client_auth: [client_secret_post, client_secret_basic, private_key_jwt, none]\n  id_token_signing: [RS256]\nschemes:\n- name: openid_connect\n  type: openIdConnect\n  openIdConnectUrl: https://gateway-portal.hub-verify.innovation.interac.ca/.well-known/openid-configuration\n  issuer: https://gateway-portal.hub-verify.innovation.interac.ca/\n  sources: [well-known/interac-openid-configuration.json]\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth\n\
  \    tokenUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token\n    pushedAuthorizationRequestUrl: https://gateway-portal.hub-verify.innovation.interac.ca/auth/par\n    refreshUrl: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token\n  grant_types_supported: [authorization_code, implicit, client_credentials, refresh_token]\nendpoints:\n  authorization_endpoint: https://gateway-portal.hub-verify.innovation.interac.ca/auth\n  pushed_authorization_request_endpoint: https://gateway-portal.hub-verify.innovation.interac.ca/auth/par\n  token_endpoint: https://gateway-portal.hub-verify.innovation.interac.ca/oauth2/token\n  userinfo_endpoint: https://gateway-portal.hub-verify.innovation.interac.ca/userinfo\n  jwks_uri: https://gateway-portal.hub-verify.innovation.interac.ca/.well-known/jwks.json\nnotes: >-\n  Relying parties authenticate with the OAuth 2.0 / OpenID Connect Authorization\n  Code Grant. The authorization request is carried either as a signed\
  \ JWT request\n  object on GET /auth or, preferably, via a back-channel Pushed Authorization\n  Request (POST /auth/par); require_request_uri_registration and\n  request_parameter_supported are both true. Clients authenticate to the token\n  endpoint with private_key_jwt (a client assertion signed by the RP's RSA key,\n  published at the RP's own JWKS URL) or client_secret_post/basic. id_tokens are\n  signed RS256. Verified claims are retrieved from GET /userinfo with the bearer\n  access token. Production issuer/endpoints are provisioned at partner onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interac/refs/heads/main/authentication/interac-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Financial Services
- Payments
- Canada
- Interac
- Digital Identity
- Verification
- Open Banking
- Consumer-Driven Banking
- Infrastructure
---
