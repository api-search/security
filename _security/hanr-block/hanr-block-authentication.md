---
anonymous_access: false
api_key_in: []
auth_types: []
description: H&R Block runs a first-party PingFederate OAuth 2.0 / OpenID Connect authorization server at https://login.hrblock.com and publishes its full discovery metadata anonymously. This profile is read directly from that document plus a live fetch of the advertised JWKS. No OpenAPI exists for the record, so nothing here is derived from a spec — every value below came off the wire on 2026-09-14.
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Hanr Block Authentication
name_suffix: Authentication
oauth_flows: []
overview: H&R Block declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: H&R Block
provider_slug: hanr-block
scheme_count: 1
schemes:
- claims_supported:
  - sub
  - entryUUID
  - givenName
  - mail
  - sn
  client_authentication:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - none
  description: Authorization server fronting MyBlock and the H&R Block digital properties. Registration, token, introspection and revocation endpoints are all advertised.
  endpoints:
    authorization: https://login.hrblock.com/as/authorization.oauth2
    backchannel_authentication: https://login.hrblock.com/as/bc-auth.ciba
    device_authorization: https://login.hrblock.com/as/device_authz.oauth2
    introspection: https://login.hrblock.com/as/introspect.oauth2
    jwks_uri: https://login.hrblock.com/pf/JWKS
    pushed_authorization_request: https://login.hrblock.com/as/par.oauth2
    registration: https://login.hrblock.com/as/clients.oauth2
    revocation: https://login.hrblock.com/as/revoke_token.oauth2
    token: https://login.hrblock.com/as/token.oauth2
    userinfo: https://login.hrblock.com/idp/userinfo.openid
  flows:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - device_code
  - token_exchange
  - jwt_bearer
  - saml2_bearer
  - ciba
  id: hrblock_oauth2
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - PS256
  - PS384
  - PS512
  - HS256
  - HS384
  - HS512
  - none
  name: H&R Block OAuth 2.0 / OpenID Connect
  pkce:
    methods:
    - S256
    - plain
    supported: true
  require_pushed_authorization_requests: false
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  subject_types:
  - public
  - pairwise
  type: oauth2
slug: hanr-block-authentication
source_filename: hanr-block-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://login.hrblock.com/.well-known/openid-configuration\nprovider: H&R Block\nproviderId: hanr-block\ndescription: >-\n  H&R Block runs a first-party PingFederate OAuth 2.0 / OpenID Connect authorization\n  server at https://login.hrblock.com and publishes its full discovery metadata\n  anonymously. This profile is read directly from that document plus a live fetch of the\n  advertised JWKS. No OpenAPI exists for the record, so nothing here is derived from a\n  spec — every value below came off the wire on 2026-09-14.\nownership: >-\n  The issuer is https://login.hrblock.com, a hrblock.com host, and the custom scopes it\n  advertises (hrbGuaid, hrbUcid) are H&R Block internal identifiers. First-party.\nissuer: https://login.hrblock.com\nproduct: PingFederate (Ping Identity)\nschemes:\n  - id: hrblock_oauth2\n    type: oauth2\n    name: H&R Block OAuth 2.0 / OpenID Connect\n    description: >-\n      Authorization server fronting\
  \ MyBlock and the H&R Block digital properties.\n      Registration, token, introspection and revocation endpoints are all advertised.\n    endpoints:\n      authorization: https://login.hrblock.com/as/authorization.oauth2\n      token: https://login.hrblock.com/as/token.oauth2\n      userinfo: https://login.hrblock.com/idp/userinfo.openid\n      jwks_uri: https://login.hrblock.com/pf/JWKS\n      registration: https://login.hrblock.com/as/clients.oauth2\n      introspection: https://login.hrblock.com/as/introspect.oauth2\n      revocation: https://login.hrblock.com/as/revoke_token.oauth2\n      device_authorization: https://login.hrblock.com/as/device_authz.oauth2\n      pushed_authorization_request: https://login.hrblock.com/as/par.oauth2\n      backchannel_authentication: https://login.hrblock.com/as/bc-auth.ciba\n    flows:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - device_code\n      - token_exchange\n\
  \      - jwt_bearer\n      - saml2_bearer\n      - ciba\n    client_authentication:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - tls_client_auth\n      - none\n    pkce:\n      supported: true\n      methods:\n        - S256\n        - plain\n    response_types:\n      - code\n      - token\n      - id_token\n      - code token\n      - code id_token\n      - token id_token\n      - code token id_token\n    subject_types:\n      - public\n      - pairwise\n    id_token_signing_algs:\n      - RS256\n      - RS384\n      - RS512\n      - ES256\n      - ES384\n      - ES512\n      - PS256\n      - PS384\n      - PS512\n      - HS256\n      - HS384\n      - HS512\n      - none\n    claims_supported:\n      - sub\n      - entryUUID\n      - givenName\n      - mail\n      - sn\n    require_pushed_authorization_requests: false\njwks:\n  url: https://login.hrblock.com/pf/JWKS\n  status: 200\n  key_count: 24\n  key_types:\n\
  \    - RSA\n    - EC\n  fetched: '2026-09-14'\ngaps:\n  - >-\n    No human-readable authentication documentation is reachable: developer.hrblock.com and\n    apiportal.hrblock.com resolve but refuse connections from the public internet, so the\n    discovery document is the only auth reference an integrator can read.\n  - >-\n    `none` appears in both id_token_signing_alg_values_supported and\n    token_endpoint_auth_methods_supported. That is the PingFederate default advertisement,\n    not necessarily an enabled client policy, but it is what the published metadata says.\nx-evidence:\n  - url: https://login.hrblock.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - url: https://login.hrblock.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - url: https://login.hrblock.com/pf/JWKS\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanr-block/refs/heads/main/authentication/hanr-block-authentication.yml
summary_line: 1 scheme
tags:
- Tax Preparation
- Financial-Services
- Fortune 1000
- Identity
- Authentication
- OpenID Connect
- Consumer Software
---
