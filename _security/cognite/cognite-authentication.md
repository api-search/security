---
api_key_in: []
api_specs:
- filename: cognite-data-fusion-api.yaml
  format: yaml
  label: Cognite Data Fusion API
  slug: cognite-data-fusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/openapi/cognite-data-fusion-api.yaml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Cognite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cognite secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cognite
provider_slug: cognite
scheme_count: 4
schemes:
- bearerFormat: OpenID Connect or OAuth2 token
  description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  name: oidc-token
  scheme: bearer
  sources:
  - openapi/cognite-data-fusion-api.json
  - openapi/cognite-data-fusion-api.yaml
  type: http
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://your-idps.token.url/
  name: oauth2-client-credentials
  sources:
  - openapi/cognite-data-fusion-api.json
  - openapi/cognite-data-fusion-api.yaml
  type: oauth2
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - authorizationUrl: https://your-idps.authorization.url/
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://your-idps.token.url/
  name: oauth2-auth-code
  sources:
  - openapi/cognite-data-fusion-api.json
  - openapi/cognite-data-fusion-api.yaml
  type: oauth2
- description: 'Access token issued by the Cognite authorization server, and valid for the target organization. The token must

    be an OpenID Connect token, and it can be obtained by performing an OIDC login flow toward `auth.cognite.com`.

    This is a single URL for all CDF organizations.'
  name: org-oidc-token
  openIdConnectUrl: https://auth.cognite.com/.well-known/openid-configuration
  sources:
  - openapi/cognite-data-fusion-api.json
  - openapi/cognite-data-fusion-api.yaml
  type: openIdConnect
slug: cognite-authentication
source_filename: cognite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognite-data-fusion-api.json, openapi/cognite-data-fusion-api.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oidc-token\n  type: http\n  scheme: bearer\n  bearerFormat: OpenID Connect or OAuth2 token\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n- name: oauth2-client-credentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-idps.token.url/\n    scopes: 1\n  description:\
  \ Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n- name: oauth2-auth-code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-idps.authorization.url/\n    tokenUrl: https://your-idps.token.url/\n    scopes: 1\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the\
  \ identity provider.\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n- name: org-oidc-token\n  type: openIdConnect\n  openIdConnectUrl: https://auth.cognite.com/.well-known/openid-configuration\n  description: |-\n    Access token issued by the Cognite authorization server, and valid for the target organization. The token must\n    be an OpenID Connect token, and it can be obtained by performing an OIDC login flow toward `auth.cognite.com`.\n    This is a single URL for all CDF organizations.\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/authentication/cognite-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Industrial IoT
- Manufacturing
- Industrial Data
- Digital Twin
- Asset Management
- Time Series
- Industrial AI
---
