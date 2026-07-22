---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Envisagenow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Envisagenow secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Envisagenow
provider_slug: envisagenow
scheme_count: 2
schemes:
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://community.envisagenow.com/cares
  name: openIdConnect
  openIdConnectUrl: https://community.envisagenow.com/.well-known/openid-configuration
  sources:
  - well-known/envisagenow-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
- authorization_endpoint: https://community.envisagenow.com/cares/services/oauth2/authorize
  introspection_endpoint: https://community.envisagenow.com/cares/services/oauth2/introspect
  jwks_uri: https://community.envisagenow.com/cares/id/keys
  name: oauth2
  registration_endpoint: https://community.envisagenow.com/cares/services/oauth2/register
  response_types_supported:
  - code
  - token
  - token id_token
  revocation_endpoint: https://community.envisagenow.com/cares/services/oauth2/revoke
  sources:
  - well-known/envisagenow-openid-configuration.json
  token_endpoint: https://community.envisagenow.com/cares/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
  userinfo_endpoint: https://community.envisagenow.com/cares/services/oauth2/userinfo
slug: envisagenow-authentication
source_filename: envisagenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://community.envisagenow.com/.well-known/openid-configuration\nnotes: >-\n  Envisage Technologies exposes no public developer API. The one publicly\n  discoverable auth surface is the Acadis Readiness Community identity provider\n  (Salesforce Experience Cloud), whose OIDC discovery document is served at\n  community.envisagenow.com/.well-known/openid-configuration. The schemes below\n  are read verbatim from that document.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode, implicit]\n  issuer: https://community.envisagenow.com/cares\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://community.envisagenow.com/.well-known/openid-configuration\n  issuer: https://community.envisagenow.com/cares\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  sources: [well-known/envisagenow-openid-configuration.json]\n- name: oauth2\n\
  \  type: oauth2\n  authorization_endpoint: https://community.envisagenow.com/cares/services/oauth2/authorize\n  token_endpoint: https://community.envisagenow.com/cares/services/oauth2/token\n  revocation_endpoint: https://community.envisagenow.com/cares/services/oauth2/revoke\n  introspection_endpoint: https://community.envisagenow.com/cares/services/oauth2/introspect\n  userinfo_endpoint: https://community.envisagenow.com/cares/services/oauth2/userinfo\n  registration_endpoint: https://community.envisagenow.com/cares/services/oauth2/register\n  jwks_uri: https://community.envisagenow.com/cares/id/keys\n  response_types_supported: [code, token, \"token id_token\"]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n  sources: [well-known/envisagenow-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envisagenow/refs/heads/main/authentication/envisagenow-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Public Safety
- Training
- Compliance
- Performance Management
- Law Enforcement
- First Responders
- Government
- SaaS
---
