---
api_key_in: []
api_specs:
- filename: unicamp-edat-data-api-openapi.yml
  format: yaml
  label: EDAT Data Platform API
  slug: edat-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unicamp/refs/heads/main/openapi/unicamp-edat-data-api-openapi.yml
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Unicamp Edat Oidc Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Campinas secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Campinas
provider_slug: unicamp
scheme_count: 1
schemes:
- description: OIDC authorization-code flow with PKCE (S256 offered). Declared as DEFAULT_AUTH_URL in the catalogo.dados.unicamp.br runtime config and enforced on api.dados.unicamp.br - an unauthenticated GET of /suporte/public/sistemas returns 401 {"message":"Unauthorized"}.
  name: edatOidc
  sources:
  - https://seguranca.dados.unicamp.br/realms/edat/.well-known/openid-configuration
  - https://catalogo.dados.unicamp.br/env.js
  type: openIdConnect
slug: unicamp-edat-oidc-authentication
source_filename: unicamp-edat-oidc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://seguranca.dados.unicamp.br/realms/edat/.well-known/openid-configuration\nnote: >-\n  Read directly from Unicamp's own OpenID Connect discovery document (HTTP 200, 6,717 bytes,\n  probed 2026-09-01). The authorization server is a Keycloak deployment operated by Unicamp on\n  its own registrable domain and is the credential authority for the EDAT data platform\n  (catalogo.dados.unicamp.br, apoio.dados.unicamp.br, api.dados.unicamp.br). It is separate from\n  Unicamp's SAML/Shibboleth identity provider registered in the CAFe federation.\nx-operator: institution\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\nissuer: https://seguranca.dados.unicamp.br/realms/edat\ndiscovery: https://seguranca.dados.unicamp.br/realms/edat/.well-known/openid-configuration\nendpoints:\n  authorization: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/auth\n  token: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/token\n\
  \  userinfo: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/userinfo\n  jwks: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/certs\n  introspection: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/token/introspect\n  revocation: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/revoke\n  end_session: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/logout\n  device_authorization: https://seguranca.dados.unicamp.br/realms/edat/protocol/openid-connect/auth/device\n  dynamic_client_registration: https://seguranca.dados.unicamp.br/realms/edat/clients-registrations/openid-connect\nschemes:\n- name: edatOidc\n  type: openIdConnect\n  description: >-\n    OIDC authorization-code flow with PKCE (S256 offered). Declared as DEFAULT_AUTH_URL in the\n    catalogo.dados.unicamp.br runtime config and enforced on api.dados.unicamp.br - an\n    unauthenticated GET of /suporte/public/sistemas\
  \ returns 401 {\"message\":\"Unauthorized\"}.\n  sources:\n  - https://seguranca.dados.unicamp.br/realms/edat/.well-known/openid-configuration\n  - https://catalogo.dados.unicamp.br/env.js\ngrant_types:\n- authorization_code\n- client_credentials\n- implicit\n- password\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:uma-ticket\n- urn:openid:params:grant-type:ciba\ntoken_endpoint_auth_methods:\n- private_key_jwt\n- client_secret_basic\n- client_secret_post\n- tls_client_auth\n- client_secret_jwt\npkce_methods:\n- S256\n- plain\nid_token_signing_algs:\n- RS256\n- ES256\n- PS256\n- EdDSA\n- HS256\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicamp/refs/heads/main/authentication/unicamp-edat-oidc-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Public Research University
- Brazil
- Latin America
- Research Data
- Open Data
- Research Repository
- Identity Federation
- OAI-PMH
- Dataverse
- Course Catalog
---
