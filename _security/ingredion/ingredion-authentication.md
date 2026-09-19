---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Ingredion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ingredion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ingredion
provider_slug: ingredion
scheme_count: 2
schemes:
- description: OpenID Connect 1.0 on the MyIngredion customer portal.
  endpoints:
    authorization: https://myingredion.com/services/oauth2/authorize
    end_session: https://myingredion.com/services/auth/idp/oidc/logout
    introspection: https://myingredion.com/services/oauth2/introspect
    jwks_uri: https://myingredion.com/id/keys
    registration: https://myingredion.com/services/oauth2/register
    revocation: https://myingredion.com/services/oauth2/revoke
    token: https://myingredion.com/services/oauth2/token
    userinfo: https://myingredion.com/services/oauth2/userinfo
  id: openIdConnect
  issuer: https://myingredion.com
  openIdConnectUrl: https://myingredion.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 authorization code with refresh. grant_types_supported declares ONLY authorization_code and refresh_token — there is no client_credentials grant, so there is no documented machine-to-machine path for an agent or a customer's own system.
  flows:
    authorizationCode:
      authorizationUrl: https://myingredion.com/services/oauth2/authorize
      refreshUrl: https://myingredion.com/services/oauth2/token
      tokenUrl: https://myingredion.com/services/oauth2/token
  id: oauth2
  type: oauth2
slug: ingredion-authentication
source_filename: ingredion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://myingredion.com/.well-known/openid-configuration\nnote: >-\n  Ingredion publishes no developer portal, no API reference and no OpenAPI, so there are no\n  securitySchemes to derive from. The ONLY machine-readable authentication description the\n  company serves anonymously is the OpenID Connect discovery document on its MyIngredion\n  customer portal. Everything below is read verbatim from that document — nothing is inferred.\n  This describes access to the CUSTOMER PORTAL, not to a published Ingredion API product.\noperator: >-\n  The portal runs on Salesforce Experience Cloud under Ingredion's own domain and Salesforce\n  org (00D30000000MNMR). The issuer, and every endpoint, is https://myingredion.com — an\n  Ingredion-controlled host — but the authentication surface itself is Salesforce platform\n  infrastructure, not an Ingredion-authored contract.\nschemes:\n  - id: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl:\
  \ https://myingredion.com/.well-known/openid-configuration\n    issuer: https://myingredion.com\n    description: OpenID Connect 1.0 on the MyIngredion customer portal.\n    endpoints:\n      authorization: https://myingredion.com/services/oauth2/authorize\n      token: https://myingredion.com/services/oauth2/token\n      userinfo: https://myingredion.com/services/oauth2/userinfo\n      revocation: https://myingredion.com/services/oauth2/revoke\n      introspection: https://myingredion.com/services/oauth2/introspect\n      registration: https://myingredion.com/services/oauth2/register\n      end_session: https://myingredion.com/services/auth/idp/oidc/logout\n      jwks_uri: https://myingredion.com/id/keys\n  - id: oauth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://myingredion.com/services/oauth2/authorize\n        tokenUrl: https://myingredion.com/services/oauth2/token\n        refreshUrl: https://myingredion.com/services/oauth2/token\n  \
  \  description: >-\n      OAuth 2.0 authorization code with refresh. grant_types_supported declares ONLY\n      authorization_code and refresh_token — there is no client_credentials grant, so there\n      is no documented machine-to-machine path for an agent or a customer's own system.\ncharacteristics:\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code, token, token id_token]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n  code_challenge_methods_supported: [S256]\n  pkce: true\n  dpop_supported: true\n  dpop_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512, EdDSA]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  dynamic_client_registration: true\n  frontchannel_logout_supported: true\napi_keys: false\nmtls: false\ndocs: null\ndocs_note: >-\n  No public authentication documentation exists. Ingredion publishes no developer\
  \ portal;\n  the portal sign-in at https://myingredion.com/s/login/ is customer-account only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingredion/refs/heads/main/authentication/ingredion-authentication.yml
summary_line: 2 schemes
tags:
- Fortune 500
- Food and Beverage
- Ingredients
- Food Manufacturing
- Agriculture
- Plant-Based Proteins
- Specialty Chemicals
- Consumer Packaged Goods
---
