---
api_key_in: []
api_specs:
- filename: devoted-patient-access-openapi.json
  format: json
  label: Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/openapi/devoted-patient-access-openapi.json
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Devoted Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Devoted Health secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Devoted Health
provider_slug: devoted
scheme_count: 2
schemes:
- authorization_endpoint: https://login.devoted.com/authorize
  issuer: https://login.devoted.com/
  jwks_uri: https://login.devoted.com/.well-known/jwks.json
  name: OpenIDConnect
  openIdConnectUrl: https://login.devoted.com/.well-known/openid-configuration
  sources:
  - well-known/devoted-openid-configuration.json
  token_endpoint: https://login.devoted.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://login.devoted.com/userinfo
- flows:
  - authorizationUrl: https://login.devoted.com/authorize
    flow: authorizationCode
    scope_ref: scopes/devoted-scopes.yml
    tokenUrl: https://login.devoted.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.devoted.com/oauth/token
  name: OAuth2
  sources:
  - well-known/devoted-openid-configuration.json
  type: oauth2
slug: devoted-authentication
source_filename: devoted-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.devoted.com/developers/\ndocs: https://www.devoted.com/developers/\nnotes: >-\n  Devoted Health's member-facing FHIR APIs (Patient Access) require member\n  authorization via OAuth 2.0 / OpenID Connect, per the CMS Interoperability and\n  Patient Access rule (21st Century Cures Act). The authorization server is an\n  Auth0 tenant published at https://login.devoted.com/.well-known/openid-configuration.\n  Third-party applications register with Devoted's interoperability team\n  (interop@devoted.com) and receive a client_id/client_secret via Virtru-encrypted\n  email. The non-member Provider & Pharmacy Directory and Plan Coverage & Formularies\n  FHIR APIs are public and do not require member authorization.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  registration: manual (app registration form + interop team review)\nschemes:\n- name: OpenIDConnect\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://login.devoted.com/.well-known/openid-configuration\n  issuer: https://login.devoted.com/\n  authorization_endpoint: https://login.devoted.com/authorize\n  token_endpoint: https://login.devoted.com/oauth/token\n  userinfo_endpoint: https://login.devoted.com/userinfo\n  jwks_uri: https://login.devoted.com/.well-known/jwks.json\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  sources:\n  - well-known/devoted-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.devoted.com/authorize\n    tokenUrl: https://login.devoted.com/oauth/token\n    scope_ref: scopes/devoted-scopes.yml\n  - flow: clientCredentials\n    tokenUrl: https://login.devoted.com/oauth/token\n  sources:\n  - well-known/devoted-openid-configuration.json\napis:\n- name: Patient Access API\n  requires_member_authorization: true\n  base_url:\
  \ https://api.prod.devoted.com/fhir\n- name: Provider & Pharmacy Directory API\n  requires_member_authorization: false\n  base_url: https://fhir.devoted.com/fhir\n- name: Plan Coverage & Formularies API\n  requires_member_authorization: false\n  base_url: https://fhir.devoted.com/fhir\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/authentication/devoted-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Healthcare
- Medicare Advantage
- Health Insurance
- FHIR
- Interoperability
- CMS Patient Access
- Payer
---
