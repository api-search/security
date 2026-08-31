---
api_key_in: []
api_specs:
- filename: tsb-bank-atm-api-openapi.yml
  format: yaml
  label: TSB Bank ATM API
  slug: tsb-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-atm-api-openapi.yml
- filename: tsb-bank-authorization-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Authorization Server APIs API
  slug: tsb-bank-authorization-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-authorization-server-apis-api-openapi.yml
- filename: tsb-bank-bca-api-openapi.yml
  format: yaml
  label: TSB Bank BCA API
  slug: tsb-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-bca-api-openapi.yml
- filename: tsb-bank-branch-api-openapi.yml
  format: yaml
  label: TSB Bank Branch API
  slug: tsb-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-branch-api-openapi.yml
- filename: tsb-bank-ccc-api-openapi.yml
  format: yaml
  label: TSB Bank CCC API
  slug: tsb-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-ccc-api-openapi.yml
- filename: tsb-bank-pca-api-openapi.yml
  format: yaml
  label: TSB Bank PCA API
  slug: tsb-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-pca-api-openapi.yml
- filename: tsb-bank-resource-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Resource Server APIs API
  slug: tsb-bank-resource-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-resource-server-apis-api-openapi.yml
- filename: tsb-bank-sme-api-openapi.yml
  format: yaml
  label: TSB Bank SME API
  slug: tsb-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-sme-api-openapi.yml
- filename: tsb-bank-token-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Token Server APIs API
  slug: tsb-bank-token-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-token-server-apis-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Tsb Bank Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- authorizationCode
- refreshToken
overview: TSB Bank secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, authorizationCode, and refreshToken flow(s).
provider_name: TSB Bank
provider_slug: tsb-bank
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize
    flow: implicit
    scopes: 5
  - authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://apis.tsb.co.uk/auth/oauth/v2/token
  name: OAuth2
  sources:
  - openapi/tsb-bank-oauth-server-openapi.json
  - well-known/tsb-bank-openid-configuration.json
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  - HS256
  issuer: https://apis.tsb.co.uk:8443
  jwks_uri: https://apis.tsb.co.uk/openid/connect/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://apis.tsb.co.uk/.well-known/openid-configuration
  registration_endpoint: https://apis.tsb.co.uk/openid/connect/register
  sources:
  - well-known/tsb-bank-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://apis.tsb.co.uk/openid/connect/v1/userinfo
- description: OBIE FAPI security profile requires mutual-TLS (eIDAS QWAC/OBIE transport certificate) between the TPP and TSB for the Read/Write services.
  name: mutualTLS
  sources:
  - obie-security-profile
  type: mutualTLS
slug: tsb-bank-authentication
source_filename: tsb-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/tsb-bank-oauth-server-openapi.json\ndocs: https://apis.tsb.co.uk/.well-known/openid-configuration\nnotes: >-\n  Enriched from TSB's live OpenID Provider discovery document. TSB runs a Curity\n  OAuth Toolkit (OTK) server as its OpenID Provider. The unauthenticated Open\n  Data API carries no security scheme (public reference data). The FAPI-secured\n  OBIE Read/Write services (AIS/PIS/CBPII) require OAuth2/OIDC with mutual-TLS\n  client authentication, request-object signing, and PSD2 strong customer\n  authentication, and are gated behind developer-portal onboarding with\n  OBIE/eIDAS certificates.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [implicit, authorizationCode, refreshToken]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  strong_customer_authentication: true\n  fapi: true\nschemes:\n- name: OAuth2\n\
  \  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize\n    scopes: 5\n  - flow: authorizationCode\n    authorizationUrl: https://apis.tsb.co.uk/auth/oauth/v2/authorize\n    tokenUrl: https://apis.tsb.co.uk/auth/oauth/v2/token\n  sources: [openapi/tsb-bank-oauth-server-openapi.json, well-known/tsb-bank-openid-configuration.json]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://apis.tsb.co.uk/.well-known/openid-configuration\n  issuer: https://apis.tsb.co.uk:8443\n  userinfo_endpoint: https://apis.tsb.co.uk/openid/connect/v1/userinfo\n  jwks_uri: https://apis.tsb.co.uk/openid/connect/jwks.json\n  registration_endpoint: https://apis.tsb.co.uk/openid/connect/register\n  id_token_signing_alg_values_supported: [RS256, HS256]\n  sources: [well-known/tsb-bank-openid-configuration.json]\n- name: mutualTLS\n  type: mutualTLS\n  description: >-\n    OBIE FAPI security profile requires mutual-TLS (eIDAS QWAC/OBIE\
  \ transport\n    certificate) between the TPP and TSB for the Read/Write services.\n  sources: [obie-security-profile]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/authentication/tsb-bank-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech
---
