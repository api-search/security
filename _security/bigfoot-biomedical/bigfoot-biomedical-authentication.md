---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Bigfoot Biomedical Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Bigfoot Biomedical secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Bigfoot Biomedical
provider_slug: bigfoot-biomedical
scheme_count: 1
schemes:
- endpoints:
    authorization: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize
    end_session: https://clinichub.bigfootbiomedical.com/services/auth/idp/oidc/logout
    introspection: https://clinichub.bigfootbiomedical.com/services/oauth2/introspect
    jwks: https://clinichub.bigfootbiomedical.com/id/keys
    registration: https://clinichub.bigfootbiomedical.com/services/oauth2/register
    revocation: https://clinichub.bigfootbiomedical.com/services/oauth2/revoke
    token: https://clinichub.bigfootbiomedical.com/services/oauth2/token
    userinfo: https://clinichub.bigfootbiomedical.com/services/oauth2/userinfo
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://clinichub.bigfootbiomedical.com
  name: bigfoot-clinic-hub-oidc
  openIdConnectUrl: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration
  platform: Salesforce Experience Cloud
  response_types_supported:
  - code
  - token
  - token id_token
  scopes: scopes/bigfoot-biomedical-scopes.yml
  sources:
  - well-known/bigfoot-biomedical-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: bigfoot-biomedical-authentication
source_filename: bigfoot-biomedical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration\nnote: >-\n  Bigfoot Biomedical publishes no API and no developer authentication documentation. The\n  only machine-readable authentication surface reachable on a Bigfoot-owned host is the\n  OpenID Connect discovery document for the Bigfoot Clinic Hub healthcare-professional\n  portal, which runs on Salesforce Experience Cloud. The endpoints and scopes below are\n  therefore Salesforce platform identity endpoints scoped to Bigfoot's org, not the\n  authentication contract of a Bigfoot product API. No Bigfoot API key, bearer token, or\n  mTLS scheme is documented anywhere on the provider's public surface.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  surface: HCP portal identity provider only — no product API behind it\nschemes:\n- name: bigfoot-clinic-hub-oidc\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration\n  issuer: https://clinichub.bigfootbiomedical.com\n  platform: Salesforce Experience Cloud\n  endpoints:\n    authorization: https://clinichub.bigfootbiomedical.com/services/oauth2/authorize\n    token: https://clinichub.bigfootbiomedical.com/services/oauth2/token\n    userinfo: https://clinichub.bigfootbiomedical.com/services/oauth2/userinfo\n    revocation: https://clinichub.bigfootbiomedical.com/services/oauth2/revoke\n    introspection: https://clinichub.bigfootbiomedical.com/services/oauth2/introspect\n    registration: https://clinichub.bigfootbiomedical.com/services/oauth2/register\n    end_session: https://clinichub.bigfootbiomedical.com/services/auth/idp/oidc/logout\n    jwks: https://clinichub.bigfootbiomedical.com/id/keys\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  scopes: scopes/bigfoot-biomedical-scopes.yml\n  sources:\n  - well-known/bigfoot-biomedical-openid-configuration.json\nx-evidence:\n- url: https://clinichub.bigfootbiomedical.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-07'\n- url: https://www.bigfootbiomedical.com/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-08-07'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigfoot-biomedical/refs/heads/main/authentication/bigfoot-biomedical-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Diabetes
- Insulin Management
- Continuous Glucose Monitoring
- Connected Devices
- Acquired
---
