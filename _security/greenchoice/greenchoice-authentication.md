---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Greenchoice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greenchoice declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Greenchoice
provider_slug: greenchoice
scheme_count: 1
schemes:
- authorization_response_iss_parameter_supported: true
  ciba:
    supported: true
    token_delivery_modes:
    - poll
    user_code_parameter_supported: true
  client_authentication:
  - client_secret_basic
  - client_secret_post
  dpop:
    signing_algs:
    - RS256
    - RS384
    - RS512
    - PS256
    - PS384
    - PS512
    - ES256
    - ES384
    - ES512
    supported: true
  dynamic_client_registration:
    note: No registration_endpoint is advertised in the discovery document, so RFC 7591 dynamic client registration is not offered. Clients are registered out of band by Greenchoice (the portal uses client_id app-mijngreenchoice).
    supported: false
  endpoints:
    authorization: https://sso.greenchoice.nl/connect/authorize
    backchannel_authentication: https://sso.greenchoice.nl/connect/ciba
    check_session_iframe: https://sso.greenchoice.nl/connect/checksession
    device_authorization: https://sso.greenchoice.nl/connect/deviceauthorization
    end_session: https://sso.greenchoice.nl/connect/endsession
    introspection: https://sso.greenchoice.nl/connect/introspect
    jwks: https://sso.greenchoice.nl/.well-known/openid-configuration/jwks
    pushed_authorization_request: https://sso.greenchoice.nl/connect/par
    revocation: https://sso.greenchoice.nl/connect/revocation
    token: https://sso.greenchoice.nl/connect/token
    userinfo: https://sso.greenchoice.nl/connect/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - soft_login_id
  - accountless_soft_login_id
  - soft_login_access
  - trusted-client
  - windows
  id_token_signing_algs:
  - RS256
  issuer: https://sso.greenchoice.nl
  logout:
    backchannel_logout_session_supported: true
    backchannel_logout_supported: true
    frontchannel_logout_session_supported: true
    frontchannel_logout_supported: true
  name: oidc_authorization_code
  non_standard_grant_note: Five of the eleven advertised grant types are vendor/bespoke rather than registered OAuth 2.0 grants. They are recorded verbatim because the discovery document advertises them; Greenchoice publishes no documentation for them, so their semantics are unknown to a public reader.
  non_standard_grant_types:
  - soft_login_id
  - accountless_soft_login_id
  - soft_login_access
  - trusted-client
  - windows
  openIdConnectUrl: https://sso.greenchoice.nl/.well-known/openid-configuration
  par:
    required: false
    supported: true
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  prompt_values:
  - none
  - login
  - consent
  - select_account
  protocol: OpenID Connect 1.0
  request_object:
    request_parameter_supported: true
    signing_algs:
    - RS256
    - RS384
    - RS512
    - PS256
    - PS384
    - PS512
    - ES256
    - ES384
    - ES512
  response_modes:
  - form_post
  - query
  - fragment
  response_types:
  - code
  - token
  - id_token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  subject_types:
  - public
  type: openIdConnect
  userinfo_signing_algs:
  - RS256
slug: greenchoice-authentication
source_filename: greenchoice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://sso.greenchoice.nl/.well-known/openid-configuration\nnote: >-\n  Derived entirely from Greenchoice's own live OpenID Connect discovery document, fetched\n  unauthenticated on 2026-09-12 (HTTP 200, application/json). Greenchoice publishes no\n  developer portal and no API authentication documentation; this profile therefore describes\n  the identity layer behind the customer-facing surfaces (Mijn Greenchoice and the mobile\n  app), not a partner or developer API programme. Nothing here is inferred — every field is a\n  value the discovery document states about itself.\nownership: >-\n  The discovery document self-identifies as issuer https://sso.greenchoice.nl, a Greenchoice\n  registrable domain, and is reached by following the 302 that https://mijn.greenchoice.nl/\n  issues to /connect/authorize?client_id=app-mijngreenchoice. It belongs to Greenchoice.\nsurface: Customer identity / single sign-on (first-party). No public\
  \ developer API.\nschemes:\n  - name: oidc_authorization_code\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    openIdConnectUrl: https://sso.greenchoice.nl/.well-known/openid-configuration\n    issuer: https://sso.greenchoice.nl\n    endpoints:\n      authorization: https://sso.greenchoice.nl/connect/authorize\n      token: https://sso.greenchoice.nl/connect/token\n      userinfo: https://sso.greenchoice.nl/connect/userinfo\n      end_session: https://sso.greenchoice.nl/connect/endsession\n      check_session_iframe: https://sso.greenchoice.nl/connect/checksession\n      revocation: https://sso.greenchoice.nl/connect/revocation\n      introspection: https://sso.greenchoice.nl/connect/introspect\n      device_authorization: https://sso.greenchoice.nl/connect/deviceauthorization\n      backchannel_authentication: https://sso.greenchoice.nl/connect/ciba\n      pushed_authorization_request: https://sso.greenchoice.nl/connect/par\n      jwks: https://sso.greenchoice.nl/.well-known/openid-configuration/jwks\n\
  \    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:openid:params:grant-type:ciba\n      - soft_login_id\n      - accountless_soft_login_id\n      - soft_login_access\n      - trusted-client\n      - windows\n    non_standard_grant_types:\n      - soft_login_id\n      - accountless_soft_login_id\n      - soft_login_access\n      - trusted-client\n      - windows\n    non_standard_grant_note: >-\n      Five of the eleven advertised grant types are vendor/bespoke rather than registered\n      OAuth 2.0 grants. They are recorded verbatim because the discovery document advertises\n      them; Greenchoice publishes no documentation for them, so their semantics are unknown\n      to a public reader.\n    response_types:\n      - code\n      - token\n      - id_token\n      - id_token token\n      - code id_token\n      - code token\n      - code id_token token\n \
  \   response_modes: [form_post, query, fragment]\n    client_authentication: [client_secret_basic, client_secret_post]\n    pkce:\n      supported: true\n      code_challenge_methods: [plain, S256]\n    dpop:\n      supported: true\n      signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512]\n    par:\n      supported: true\n      required: false\n    ciba:\n      supported: true\n      token_delivery_modes: [poll]\n      user_code_parameter_supported: true\n    request_object:\n      request_parameter_supported: true\n      signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512]\n    id_token_signing_algs: [RS256]\n    userinfo_signing_algs: [RS256]\n    subject_types: [public]\n    prompt_values: [none, login, consent, select_account]\n    logout:\n      frontchannel_logout_supported: true\n      frontchannel_logout_session_supported: true\n      backchannel_logout_supported: true\n      backchannel_logout_session_supported: true\n    authorization_response_iss_parameter_supported:\
  \ true\n    dynamic_client_registration:\n      supported: false\n      note: >-\n        No registration_endpoint is advertised in the discovery document, so RFC 7591 dynamic\n        client registration is not offered. Clients are registered out of band by Greenchoice\n        (the portal uses client_id app-mijngreenchoice).\nscopes_reference: scopes/greenchoice-scopes.yml\napi_keys:\n  offered: false\n  note: No API key programme is published.\nmtls:\n  offered: false\ndocs:\n  - url: https://mijn.greenchoice.nl/\n    status: 200\n    note: >-\n      Customer login entry point; 302s to the authorize endpoint. There is no human-readable\n      authentication reference — this artifact is built from the machine-readable document only.\ngaps:\n  - No developer documentation describes any of these endpoints.\n  - No dynamic client registration; third parties cannot obtain a client_id.\n  - >-\n    No /.well-known/oauth-protected-resource (RFC 9728) document, so a resource server and its\n\
  \    required scopes cannot be discovered from the issuer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenchoice/refs/heads/main/authentication/greenchoice-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Electricity
- Gas
- Renewables
- Sustainability
- Netherlands
---
