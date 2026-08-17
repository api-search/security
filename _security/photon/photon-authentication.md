---
api_key_in: []
api_specs:
- filename: photon-website-api-openapi.json
  format: json
  label: Photon Website API
  slug: photon-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-website-api-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Photon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Photon secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Photon
provider_slug: photon
scheme_count: 2
schemes:
- expires_in: 86400
  flow: clientCredentials
  name: OAuth2ClientCredentials
  production:
    audience: https://api.photon.health
    issuer: https://auth.photon.health/
    jwks_uri: https://auth.photon.health/.well-known/jwks.json
    token_url: https://auth.photon.health/oauth/token
  provider: Auth0
  request_params:
  - client_id
  - client_secret
  - audience
  - grant_type
  sandbox:
    audience: https://api.neutron.health
    token_url: https://auth.neutron.health/oauth/token
  sources:
  - well-known/photon-openid-configuration.json
  - review.yml
  token_type: Bearer
  type: oauth2
- in: header
  name: BearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.photon.health/docs/authentication
  type: http
slug: photon-authentication
source_filename: photon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://docs.photon.health/docs/authentication\ndocs: https://docs.photon.health/docs/authentication\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  oauth2_flows: [clientCredentials]\n  provider: Auth0\n  notes: >-\n    Photon secures its single GraphQL endpoint with OAuth2 client-credentials\n    access tokens issued by Auth0. Tokens are presented as a Bearer token in the\n    Authorization header. Two token shapes: machine-to-machine (backend, all\n    actions except write:prescription) and user access tokens (frontend via\n    Elements; only authorized providers receive write:prescription).\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  provider: Auth0\n  production:\n    token_url: https://auth.photon.health/oauth/token\n    audience: https://api.photon.health\n    issuer: https://auth.photon.health/\n    jwks_uri: https://auth.photon.health/.well-known/jwks.json\n\
  \  sandbox:\n    token_url: https://auth.neutron.health/oauth/token\n    audience: https://api.neutron.health\n  token_type: Bearer\n  expires_in: 86400\n  request_params: [client_id, client_secret, audience, grant_type]\n  sources: [well-known/photon-openid-configuration.json, review.yml]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  sources: [https://docs.photon.health/docs/authentication]\ntoken_shapes:\n- name: Machine-to-Machine (M2M)\n  audience: backend\n  note: Obtained from the Photon app settings; can perform all actions except write:prescription.\n- name: User Access Token\n  audience: frontend\n  note: Generated from logged-in user roles (via Elements); only authorized providers get write:prescription.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/authentication/photon-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Healthcare
- United States
- e-Prescribing
- Pharmacy
- Prescription Routing
- GraphQL
- Clinical API
- Digital Health
- Benefit Check
- OAuth2
---
