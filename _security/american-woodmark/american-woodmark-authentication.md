---
api_key_in: []
auth_types: []
description: Authentication profile for American Woodmark, read directly from the live OpenID Connect discovery document its identity provider serves anonymously at id.woodmark.com. There is no OpenAPI to derive securitySchemes from and no public developer documentation, so every field below is taken verbatim from the discovery document rather than from prose.
kind: authentication
layout: security
method: probed
name: American Woodmark Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Woodmark declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: American Woodmark
provider_slug: american-woodmark
scheme_count: 3
schemes:
- bearer_format: JWT
  description: Full OpenID Connect provider. Discovery, JWKS, userinfo, session management and both front-channel and back-channel logout are advertised.
  in: header
  name: openIdConnect
  openIdConnectUrl: https://id.woodmark.com/.well-known/openid-configuration
  scheme: bearer
  type: openIdConnect
- description: OAuth 2.0 authorization server co-located with the OIDC provider. Six grant types are advertised, including client_credentials for machine-to-machine access and the RFC 8628 device authorization grant.
  flows:
    authorizationCode:
      authorizationUrl: https://id.woodmark.com/connect/authorize
      refreshUrl: https://id.woodmark.com/connect/token
      tokenUrl: https://id.woodmark.com/connect/token
    clientCredentials:
      tokenUrl: https://id.woodmark.com/connect/token
    deviceCode:
      deviceAuthorizationUrl: https://id.woodmark.com/connect/deviceauthorization
      tokenUrl: https://id.woodmark.com/connect/token
    implicit:
      authorizationUrl: https://id.woodmark.com/connect/authorize
    password:
      tokenUrl: https://id.woodmark.com/connect/token
  name: oauth2
  type: oauth2
- description: The discovery document advertises a non-standard `apikey_endpoint` at https://id.woodmark.com/api/resources/validateapikey, indicating an API key credential is validated alongside the OAuth/OIDC tokens. The key header name, format and issuance flow are NOT published — American Woodmark documents none of this publicly. Recorded because the endpoint is advertised, not because its usage is documented.
  in: header
  name: apiKey
  type: apiKey
slug: american-woodmark-authentication
source_filename: american-woodmark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://id.woodmark.com/.well-known/openid-configuration\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: American Woodmark\nproviderId: american-woodmark\ndescription: >-\n  Authentication profile for American Woodmark, read directly from the live\n  OpenID Connect discovery document its identity provider serves anonymously at\n  id.woodmark.com. There is no OpenAPI to derive securitySchemes from and no\n  public developer documentation, so every field below is taken verbatim from\n  the discovery document rather than from prose.\nownership_note: >-\n  woodmark.com is American Woodmark's own registrable domain —\n  https://www.woodmark.com/ returns 200 titled \"American Woodmark\" and\n  redirects to www.americanwoodmark.com, and github.com/AmericanWoodmark lists\n  woodmark.com as its website.\nissuer: https://id.woodmark.com\nplatform: >-\n  IdentityServer (Duende / IdentityServer4 endpoint\
  \ shape — /connect/authorize,\n  /connect/token, /connect/introspect, /connect/revocation)\nschemes:\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://id.woodmark.com/.well-known/openid-configuration\n    description: >-\n      Full OpenID Connect provider. Discovery, JWKS, userinfo, session\n      management and both front-channel and back-channel logout are advertised.\n    in: header\n    scheme: bearer\n    bearer_format: JWT\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization server co-located with the OIDC provider. Six\n      grant types are advertised, including client_credentials for\n      machine-to-machine access and the RFC 8628 device authorization grant.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://id.woodmark.com/connect/authorize\n        tokenUrl: https://id.woodmark.com/connect/token\n        refreshUrl: https://id.woodmark.com/connect/token\n      clientCredentials:\n    \
  \    tokenUrl: https://id.woodmark.com/connect/token\n      implicit:\n        authorizationUrl: https://id.woodmark.com/connect/authorize\n      password:\n        tokenUrl: https://id.woodmark.com/connect/token\n      deviceCode:\n        deviceAuthorizationUrl: https://id.woodmark.com/connect/deviceauthorization\n        tokenUrl: https://id.woodmark.com/connect/token\n  - name: apiKey\n    type: apiKey\n    in: header\n    description: >-\n      The discovery document advertises a non-standard `apikey_endpoint` at\n      https://id.woodmark.com/api/resources/validateapikey, indicating an API\n      key credential is validated alongside the OAuth/OIDC tokens. The key\n      header name, format and issuance flow are NOT published — American\n      Woodmark documents none of this publicly. Recorded because the endpoint\n      is advertised, not because its usage is documented.\nendpoints:\n  authorization: https://id.woodmark.com/connect/authorize\n  token: https://id.woodmark.com/connect/token\n\
  \  userinfo: https://id.woodmark.com/connect/userinfo\n  jwks: https://id.woodmark.com/.well-known/openid-configuration/jwks\n  introspection: https://id.woodmark.com/connect/introspect\n  revocation: https://id.woodmark.com/connect/revocation\n  end_session: https://id.woodmark.com/connect/endsession\n  check_session_iframe: https://id.woodmark.com/connect/checksession\n  device_authorization: https://id.woodmark.com/connect/deviceauthorization\n  apikey_validation: https://id.woodmark.com/api/resources/validateapikey\n  client_claims: https://id.woodmark.com/api/client/claims\n  client_credentials: https://id.woodmark.com/api/client/credentials\ngrant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\nresponse_types_supported:\n  - code\n  - token\n  - id_token\n  - id_token token\n  - code id_token\n  - code token\n  - code id_token token\nresponse_modes_supported:\n  - form_post\n\
  \  - query\n  - fragment\ntoken_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\npkce:\n  supported: true\n  code_challenge_methods_supported:\n    - plain\n    - S256\n  note: >-\n    S256 is offered, but `plain` is also still advertised. RFC 7636 §7.2 and\n    OAuth 2.1 both require S256 for public clients; advertising `plain`\n    permits a downgrade.\nid_token:\n  signing_alg_values_supported:\n    - RS256\n  subject_types_supported:\n    - public\nlogout:\n  frontchannel_logout_supported: true\n  frontchannel_logout_session_supported: true\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\ndynamic_client_registration:\n  supported: false\n  note: >-\n    No `registration_endpoint` is advertised in the discovery document, so\n    RFC 7591 dynamic client registration is not available. Clients must be\n    provisioned out of band by American Woodmark.\nobservations:\n  - >-\n    `password` (Resource Owner Password Credentials)\
  \ and `implicit` are both\n    still advertised. Both are removed in OAuth 2.1 and discouraged by the\n    OAuth Security BCP (RFC 9700).\n  - >-\n    A `TestClient` scope is advertised in scopes_supported on the production\n    issuer — see scopes/american-woodmark-scopes.yml.\n  - >-\n    No /.well-known/oauth-protected-resource is served (404), so RFC 9728\n    protected-resource metadata is absent and an agent cannot discover which\n    resource server these tokens are for.\ngaps:\n  - No public developer documentation describes how to obtain a client_id.\n  - No published scope-to-operation mapping; no API reference of any kind.\n  - No OpenAPI, AsyncAPI, GraphQL SDL, WSDL or .proto published anywhere.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-woodmark/refs/heads/main/authentication/american-woodmark-authentication.yml
summary_line: 3 schemes
tags:
- Cabinetry
- Home Products
- Construction
- Building Products
- Manufacturing
- Kitchen and Bath
- Home Improvement
- Identity
- EDI
- Supply Chain
---
