---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Picogrid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- password
- implicit
overview: Picogrid secures its APIs with oauth2, openIdConnect, and mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, password, and implicit flow(s).
provider_name: Picogrid
provider_slug: picogrid
scheme_count: 1
schemes:
- authorization_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth
  code_challenge_methods_supported:
  - S256
  - plain
  device_authorization_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth/device
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - implicit
  - password
  introspection_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token/introspect
  issuer: https://auth.legion-prod.picogrid.com/realms/legion
  jwks_uri: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/certs
  name: OAuth2
  provider: Keycloak
  realm: legion
  registration_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/clients-registrations/openid-connect
  revocation_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/revoke
  sources:
  - well-known/picogrid-oauth-authorization-server.json
  token_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: oauth2
slug: picogrid-authentication
source_filename: picogrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://legion-prod.picogrid.com/v3/.well-known/oauth-authorization-server\ndocs: https://docs.picogrid.com/reference/start\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, password, implicit]\n  identity_provider: Keycloak (realm \"legion\")\n  fine_grained_authorization: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  provider: Keycloak\n  realm: legion\n  issuer: https://auth.legion-prod.picogrid.com/realms/legion\n  authorization_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth\n  token_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token\n  jwks_uri: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/certs\n  registration_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/clients-registrations/openid-connect\n \
  \ introspection_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/revoke\n  device_authorization_endpoint: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth/device\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - implicit\n  - password\n  code_challenge_methods_supported: [S256, plain]\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  sources: [well-known/picogrid-oauth-authorization-server.json]\nnotes: >-\n  Machine-to-machine integrations authenticate with the OAuth 2.0 client\n  credentials grant against the Keycloak\
  \ \"legion\" realm; interactive apps use\n  authorization_code with PKCE (S256). Token exchange (RFC 8693), device\n  authorization grant, and mTLS-bound access tokens (tls_client_auth) are\n  supported. Integration OAuth clients are provisioned via the /v3/integrations\n  endpoints (client id/secret issuance + regeneration) and token signatures are\n  verified against the JWKS. Legion applies fine-grained authorization on top of\n  OAuth (org-scoped permissions: org:viewer/operator/admin/system-admin,\n  permission templates, grant/revoke/check/expand/trace).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picogrid/refs/heads/main/authentication/picogrid-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 1 scheme
tags:
- Company
- Data
- Defense
- Public Safety
- Systems Integration
- Sensors
- Unmanned Systems
- Command and Control
- Geospatial
- Situational Awareness
- OAuth
- Video Streaming
---
