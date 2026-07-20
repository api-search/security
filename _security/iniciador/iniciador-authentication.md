---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Iniciador Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- refreshToken
overview: Iniciador secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, and refreshToken flow(s).
provider_name: Iniciador
provider_slug: iniciador
scheme_count: 3
schemes:
- issuer: https://api.iniciador.com.br
  name: OpenFinanceBrasilOIDC
  openIdConnectUrl: https://api.iniciador.com.br/.well-known/openid-configuration
  sources:
  - well-known/iniciador-openid-configuration.json
  type: openIdConnect
- acr_values_supported:
  - urn:brasil:openbanking:loa2
  - urn:brasil:openbanking:loa3
  flows:
  - authorizationUrl: https://auth.iniciador.com.br/auth
    flow: authorizationCode
    tokenUrl: https://api-mtls.iniciador.com.br/token
  - flow: clientCredentials
    tokenUrl: https://api-mtls.iniciador.com.br/token
  grant_types_supported:
  - implicit
  - authorization_code
  - refresh_token
  - client_credentials
  jwks_uri: https://api.iniciador.com.br/jwks
  name: OAuth2
  pushed_authorization_request_endpoint: https://api-mtls.iniciador.com.br/request
  registration_endpoint: https://api-mtls.iniciador.com.br/reg
  request_object_signing_alg_values_supported:
  - PS256
  response_types_supported:
  - code id_token
  sources:
  - well-known/iniciador-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  type: oauth2
  userinfo_endpoint: https://api-mtls.iniciador.com.br/me
- description: Certificate-bound access tokens (tls_client_certificate_bound_access_tokens = true); token/userinfo/PAR/registration served on api-mtls.iniciador.com.br.
  name: mutualTLS
  sources:
  - well-known/iniciador-openid-configuration.json
  type: mutualTLS
slug: iniciador-authentication
source_filename: iniciador-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.iniciador.com.br/.well-known/openid-configuration\ndocs: https://docs.iniciador.com.br\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  profile: FAPI / Open Finance Brasil (Brasil Open Finance security profile)\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\n  - refreshToken\n  client_authentication:\n  - private_key_jwt\n  notable:\n  - mTLS-bound (certificate-bound) access tokens\n  - Pushed Authorization Requests (PAR) required\n  - PS256-signed request objects\n  - LoA2 / LoA3 (urn:brasil:openbanking) authentication contexts\nschemes:\n- name: OpenFinanceBrasilOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://api.iniciador.com.br/.well-known/openid-configuration\n  issuer: https://api.iniciador.com.br\n  sources:\n  - well-known/iniciador-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://auth.iniciador.com.br/auth\n    tokenUrl: https://api-mtls.iniciador.com.br/token\n  - flow: clientCredentials\n    tokenUrl: https://api-mtls.iniciador.com.br/token\n  response_types_supported:\n  - code id_token\n  grant_types_supported:\n  - implicit\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  request_object_signing_alg_values_supported:\n  - PS256\n  acr_values_supported:\n  - urn:brasil:openbanking:loa2\n  - urn:brasil:openbanking:loa3\n  pushed_authorization_request_endpoint: https://api-mtls.iniciador.com.br/request\n  registration_endpoint: https://api-mtls.iniciador.com.br/reg\n  jwks_uri: https://api.iniciador.com.br/jwks\n  userinfo_endpoint: https://api-mtls.iniciador.com.br/me\n  sources:\n  - well-known/iniciador-openid-configuration.json\n- name: mutualTLS\n  type: mutualTLS\n  description: Certificate-bound access tokens (tls_client_certificate_bound_access_tokens = true);\
  \ token/userinfo/PAR/registration served on api-mtls.iniciador.com.br.\n  sources:\n  - well-known/iniciador-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iniciador/refs/heads/main/authentication/iniciador-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Company
- Fintech
- Open Finance
- Open Banking
- Payments
- Pix
- Brazil
- FAPI
- OAuth
- Financial Services
---
