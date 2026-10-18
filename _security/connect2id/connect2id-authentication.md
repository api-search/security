---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Connect2Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: Connect2id declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Connect2id
provider_slug: connect2id
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://demo.c2id.com/c2id-login
    flow: authorizationCode
    tokenUrl: https://demo.c2id.com/token
  - flow: clientCredentials
    tokenUrl: https://demo.c2id.com/token
  - flow: password
    tokenUrl: https://demo.c2id.com/token
  - authorizationUrl: https://demo.c2id.com/c2id-login
    flow: implicit
  name: oauth2
  sources:
  - https://demo.c2id.com/.well-known/openid-configuration
  type: oauth2
- name: openIdConnect
  openIdConnectUrl: https://demo.c2id.com/.well-known/openid-configuration
  type: openIdConnect
slug: connect2id-authentication
source_filename: connect2id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://demo.c2id.com/.well-known/openid-configuration\nnote: Profile of the Connect2id server as exposed on the public demo issuer; product\n  endpoints are deployment-specific.\nissuer: https://demo.c2id.com\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://demo.c2id.com/c2id-login\n    tokenUrl: https://demo.c2id.com/token\n  - flow: clientCredentials\n    tokenUrl: https://demo.c2id.com/token\n  - flow: password\n    tokenUrl: https://demo.c2id.com/token\n  - flow: implicit\n    authorizationUrl: https://demo.c2id.com/c2id-login\n  sources:\n  - https://demo.c2id.com/.well-known/openid-configuration\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://demo.c2id.com/.well-known/openid-configuration\noidc_discovery: https://demo.c2id.com/.well-known/openid-configuration\nendpoints:\n  authorization_endpoint: https://demo.c2id.com/c2id-login\n\
  \  token_endpoint: https://demo.c2id.com/token\n  registration_endpoint: https://demo.c2id.com/clients\n  introspection_endpoint: https://demo.c2id.com/token/introspect\n  revocation_endpoint: https://demo.c2id.com/token/revoke\n  pushed_authorization_request_endpoint: https://demo.c2id.com/par\n  userinfo_endpoint: https://demo.c2id.com/userinfo\n  end_session_endpoint: https://demo.c2id.com/c2id-login/logout\ngrant_types:\n- implicit\n- authorization_code\n- refresh_token\n- password\n- client_credentials\n- urn:ietf:params:oauth:grant-type:jwt-bearer\nresponse_types:\n- code\n- token\n- id_token\n- id_token token\n- code id_token\n- code id_token token\ntoken_endpoint_auth_methods:\n- client_secret_basic\n- client_secret_post\n- client_secret_jwt\n- private_key_jwt\n- self_signed_tls_client_auth\n- none\ncode_challenge_methods:\n- plain\n- S256\ndocumentation: https://connect2id.com/products/server/docs/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connect2id/refs/heads/main/authentication/connect2id-authentication.yml
summary_line: 2 schemes
tags:
- Company
- OpenID Connect
- Authentication
- Identity
---
