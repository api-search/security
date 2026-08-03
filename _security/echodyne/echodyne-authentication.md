---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Echodyne Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Echodyne secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Echodyne
provider_slug: echodyne
scheme_count: 1
schemes:
- dynamic_client_registration: true
  endpoints:
    authorization: https://portal.echodyne.com/services/oauth2/authorize
    end_session: https://portal.echodyne.com/services/auth/idp/oidc/logout
    introspection: https://portal.echodyne.com/services/oauth2/introspect
    jwks: https://portal.echodyne.com/id/keys
    registration: https://portal.echodyne.com/services/oauth2/register
    revocation: https://portal.echodyne.com/services/oauth2/revoke
    token: https://portal.echodyne.com/services/oauth2/token
    userinfo: https://portal.echodyne.com/services/oauth2/userinfo
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://portal.echodyne.com
  name: EchodynePortalOIDC
  openIdConnectUrl: https://portal.echodyne.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  - token id_token
  scopes: scopes/echodyne-scopes.yml
  sources:
  - well-known/echodyne-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: echodyne-authentication
source_filename: echodyne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://portal.echodyne.com/.well-known/openid-configuration\ndocs: https://portal.echodyne.com/s/login/\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  note: 'Derived from the anonymous OIDC discovery document served by the Echodyne Customer\n    Portal (Salesforce Experience Cloud). This governs access to the customer portal — the\n    distribution point for radar software, manuals, tooling and the ATAK plugin. It does NOT\n    describe authentication to the EchoWare radar management/data API itself, which runs on\n    the operator''s own network and whose auth model is documented only inside the gated\n    portal.'\nschemes:\n- name: EchodynePortalOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://portal.echodyne.com/.well-known/openid-configuration\n  issuer: https://portal.echodyne.com\n  endpoints:\n    authorization: https://portal.echodyne.com/services/oauth2/authorize\n\
  \    token: https://portal.echodyne.com/services/oauth2/token\n    userinfo: https://portal.echodyne.com/services/oauth2/userinfo\n    revocation: https://portal.echodyne.com/services/oauth2/revoke\n    introspection: https://portal.echodyne.com/services/oauth2/introspect\n    registration: https://portal.echodyne.com/services/oauth2/register\n    end_session: https://portal.echodyne.com/services/auth/idp/oidc/logout\n    jwks: https://portal.echodyne.com/id/keys\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  subject_types_supported:\n  - public\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  dynamic_client_registration: true\n  frontchannel_logout_supported: true\n  scopes: scopes/echodyne-scopes.yml\n  sources:\n  - well-known/echodyne-openid-configuration.json\nunpublished:\n  - surface: EchoWare radar management and data API\n    reason:\
  \ 'No public authentication documentation. Radar API reference and manuals are\n      distributed through the login-gated Echodyne Customer Portal. Public technical sheets\n      describe only the transport (TCP/IP Gigabit / 10 Gbps Ethernet), not the auth model.'\n    evidence: https://www.echodyne.com/radar-systems/echoware\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://portal.echodyne.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echodyne/refs/heads/main/authentication/echodyne-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Radar
- Defense
- Government
- Critical Infrastructure
- Counter-UAS
- Drone Detection
- Sensors
- Situational Awareness
- Aerospace
- Hardware
- Public Safety
---
