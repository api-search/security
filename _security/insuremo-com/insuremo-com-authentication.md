---
anonymous_access: false
api_key_in: []
api_specs:
- filename: insuremo-com-openapi-generated.yml
  format: yaml
  label: insureMO API Platform
  slug: insuremo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insuremo-com/openapi/_ae-authored/insuremo-com-openapi-generated.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: insureMO Authentication
name_suffix: Authentication
oauth_flows: []
overview: insureMO secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: insureMO
provider_slug: insuremo-com
scheme_count: 1
schemes:
- description: 'OAuth 2.0 / OIDC served by the insureMO CAS identity service on the API gateway (issuer https://portal-gw.insuremo.com/cas). Bearer tokens are sent in the Authorization header (protected-resource metadata: bearer_methods_supported [header]).'
  flows:
    authorizationCode:
      authorizationUrl: https://portal-gw.insuremo.com/cas/oidc/authorize
      pkce: S256
      tokenUrl: https://portal-gw.insuremo.com/cas/oidc/token
    clientCredentials:
      tokenUrl: https://portal-gw.insuremo.com/cas/oidc/token
  jwks_uri: https://portal-gw.insuremo.com/cas/oidc/.well-known/jwks.json
  name: insuremoCasOidc
  scopes:
  - openid
  - profile
  - email
  sources:
  - well-known/insuremo-com-portal-gw-oauth-authorization-server.json
  - well-known/insuremo-com-portal-gw-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
slug: insuremo-com-authentication
source_filename: insuremo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: https://portal-gw.insuremo.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\nschemes:\n- name: insuremoCasOidc\n  type: oauth2\n  description: 'OAuth 2.0 / OIDC served by the insureMO CAS identity service on the API gateway (issuer https://portal-gw.insuremo.com/cas). Bearer tokens are sent in the Authorization header (protected-resource\n    metadata: bearer_methods_supported [header]).'\n  flows:\n    authorizationCode:\n      authorizationUrl: https://portal-gw.insuremo.com/cas/oidc/authorize\n      tokenUrl: https://portal-gw.insuremo.com/cas/oidc/token\n      pkce: S256\n    clientCredentials:\n      tokenUrl: https://portal-gw.insuremo.com/cas/oidc/token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  scopes:\n  - openid\n  - profile\n  - email\n  jwks_uri: https://portal-gw.insuremo.com/cas/oidc/.well-known/jwks.json\n  sources:\n \
  \ - well-known/insuremo-com-portal-gw-oauth-authorization-server.json\n  - well-known/insuremo-com-portal-gw-oauth-protected-resource.json\nnote: The first-party Postman sample (github.com/InsureMO/calling-insuremo-api-sample) calls the gateway with an access_token variable obtained from insureMO.\n"
source_yaml_url: https://artifacts.apis.io/insuremo-com/authentication/insuremo-com-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Insurance
- Artificial Intelligence
- Platform
---
