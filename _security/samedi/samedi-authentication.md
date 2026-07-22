---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Samedi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: samedi secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: samedi
provider_slug: samedi
scheme_count: 3
schemes:
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://patient.samedi.de
  name: OpenIDConnect
  openIdConnectUrl: https://patient.samedi.de/.well-known/openid-configuration
  sources:
  - well-known/samedi-openid-configuration.json
  subject_types_supported:
  - pairwise
  type: openIdConnect
- endpoints:
    introspection_endpoint: https://patient.samedi.de/oauth/introspect
    jwks_uri: https://patient.samedi.de/oauth/discovery/keys
    revocation_endpoint: https://patient.samedi.de/oauth/revoke
    userinfo_endpoint: https://patient.samedi.de/oauth/userinfo
  flows:
  - authorizationUrl: https://patient.samedi.de/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://patient.samedi.de/oauth/token
  - flow: clientCredentials
    tokenUrl: https://patient.samedi.de/oauth/token
  name: OAuth2
  sources:
  - well-known/samedi-oauth-authorization-server.json
  type: oauth2
- flows:
  - authorizationUrl: https://patient.samedi.de/api/auth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://patient.samedi.de/api/auth/v2/token
  name: BookingAPIOAuth
  sources:
  - https://github.com/samedi/omniauth-samedi
  type: oauth2
slug: samedi-authentication
source_filename: samedi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://patient.samedi.de/.well-known/openid-configuration\ndocs: https://wiki.samedi.de/display/doc/Booking+API\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\nnotes: >-\n  samedi exposes OAuth 2.0 / OpenID Connect at patient.samedi.de. Two versioned\n  OAuth surfaces are documented: the OIDC provider at /oauth/* (issuer\n  https://patient.samedi.de) and the Booking API OAuth at /api/auth/v2/* used by\n  the official omniauth-samedi strategy. API requests are authorized with a\n  Bearer access token. API credentials are requested at\n  https://patient.samedi.de/api/signup.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://patient.samedi.de/.well-known/openid-configuration\n  issuer: https://patient.samedi.de\n  id_token_signing_alg_values_supported:\
  \ [RS256]\n  subject_types_supported: [pairwise]\n  sources: ['well-known/samedi-openid-configuration.json']\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient.samedi.de/oauth/authorize\n    tokenUrl: https://patient.samedi.de/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://patient.samedi.de/oauth/token\n  endpoints:\n    revocation_endpoint: https://patient.samedi.de/oauth/revoke\n    introspection_endpoint: https://patient.samedi.de/oauth/introspect\n    userinfo_endpoint: https://patient.samedi.de/oauth/userinfo\n    jwks_uri: https://patient.samedi.de/oauth/discovery/keys\n  sources: ['well-known/samedi-oauth-authorization-server.json']\n- name: BookingAPIOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient.samedi.de/api/auth/v2/authorize\n    tokenUrl: https://patient.samedi.de/api/auth/v2/token\n  sources: ['https://github.com/samedi/omniauth-samedi']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samedi/refs/heads/main/authentication/samedi-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Healthcare
- Scheduling
- Appointments
- Booking
- Patient Engagement
- OAuth
- FHIR
- Telemedicine
- Germany
---
