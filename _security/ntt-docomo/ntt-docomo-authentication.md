---
api_key_in: []
auth_types:
- openIdConnect
description: NTT DOCOMO, Inc. publishes no REST API and therefore no OpenAPI securitySchemes. Its one anonymously discoverable authentication surface is d ACCOUNT Connect (dアカウント・コネクト), an OpenID Connect Provider fronting roughly 90 million d ACCOUNT registrations across approximately 2,000 implemented relying-party sites. This profile is read from the live OIDC discovery document plus DOCOMO's own business documentation — the integration manual and support libraries are downloadable only after an application and a DOCOMO review (審査), so the client-authentication methods, grant types and claim set are not publicly readable.
kind: authentication
layout: security
method: searched
name: Ntt Docomo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NTT Docomo secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NTT Docomo
provider_slug: ntt-docomo
scheme_count: 1
schemes:
- endpoints:
    authorization_endpoint: https://id.smt.docomo.ne.jp/cgi8/oidc/authorize
    backchannel_authentication_endpoint: null
    end_session_endpoint: null
    introspection_endpoint: null
    jwks_uri: https://fr-end.oidc.if.cilite.docomo.ne.jp/oft/external/ofrnt/v1.0/jwksget
    registration_endpoint: null
    revocation_endpoint: null
    token_endpoint: https://conf.uw.docomo.ne.jp/token
    userinfo_endpoint: https://conf.uw.docomo.ne.jp/userinfo
  flows:
  - authorizationUrl: https://id.smt.docomo.ne.jp/cgi8/oidc/authorize
    flow: authorizationCode
    note: response_types_supported is ["code"] only — implicit and hybrid are not advertised. No PKCE metadata (code_challenge_methods_supported) is published.
    tokenUrl: https://conf.uw.docomo.ne.jp/token
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  issuer: https://conf.uw.docomo.ne.jp/
  jwks:
    file: well-known/ntt-docomo-jwks.json
    keys: 1
    kid: null
    kty: RSA
    note: The single published key carries no kid and no alg member.
    use: sig
  name: d ACCOUNT Connect
  openIdConnectUrl: https://conf.uw.docomo.ne.jp/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/ntt-docomo-openid-configuration.json
  subject_types_supported:
  - pairwise
  type: openIdConnect
slug: ntt-docomo-authentication
source_filename: ntt-docomo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://conf.uw.docomo.ne.jp/.well-known/openid-configuration (HTTP 200,\n  fetched 2026-07-25, saved verbatim at\n  well-known/ntt-docomo-openid-configuration.json);\n  https://id.smt.docomo.ne.jp/src/index_business.html;\n  https://id.smt.docomo.ne.jp/src/dlogin/ctop_method.html\ndocs: https://id.smt.docomo.ne.jp/src/dlogin/ctop_method.html\ndescription: >-\n  NTT DOCOMO, Inc. publishes no REST API and therefore no OpenAPI\n  securitySchemes. Its one anonymously discoverable authentication surface is\n  d ACCOUNT Connect (dアカウント・コネクト), an OpenID Connect Provider fronting\n  roughly 90 million d ACCOUNT registrations across approximately 2,000\n  implemented relying-party sites. This profile is read from the live OIDC\n  discovery document plus DOCOMO's own business documentation — the integration\n  manual and support libraries are downloadable only after an application and\n  a DOCOMO review (審査), so the client-authentication\
  \ methods, grant types and\n  claim set are not publicly readable.\nsummary:\n  types: [openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  self_serve_credentials: false\n  gate: application + DOCOMO review (審査), ~3 business days per stage\nschemes:\n  - name: d ACCOUNT Connect\n    type: openIdConnect\n    openIdConnectUrl: https://conf.uw.docomo.ne.jp/.well-known/openid-configuration\n    issuer: https://conf.uw.docomo.ne.jp/\n    sources:\n      - well-known/ntt-docomo-openid-configuration.json\n    endpoints:\n      authorization_endpoint: https://id.smt.docomo.ne.jp/cgi8/oidc/authorize\n      token_endpoint: https://conf.uw.docomo.ne.jp/token\n      userinfo_endpoint: https://conf.uw.docomo.ne.jp/userinfo\n      jwks_uri: https://fr-end.oidc.if.cilite.docomo.ne.jp/oft/external/ofrnt/v1.0/jwksget\n      registration_endpoint: null\n      backchannel_authentication_endpoint: null\n      end_session_endpoint: null\n      revocation_endpoint: null\n      introspection_endpoint:\
  \ null\n    response_types_supported: [code]\n    subject_types_supported: [pairwise]\n    id_token_signing_alg_values_supported: [HS256, RS256]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://id.smt.docomo.ne.jp/cgi8/oidc/authorize\n        tokenUrl: https://conf.uw.docomo.ne.jp/token\n        note: >-\n          response_types_supported is [\"code\"] only — implicit and hybrid are\n          not advertised. No PKCE metadata\n          (code_challenge_methods_supported) is published.\n    jwks:\n      file: well-known/ntt-docomo-jwks.json\n      keys: 1\n      kty: RSA\n      use: sig\n      kid: null\n      note: The single published key carries no kid and no alg member.\nundeclared_in_metadata:\n  - scopes_supported\n  - grant_types_supported\n  - token_endpoint_auth_methods_supported\n  - claims_supported\n  - code_challenge_methods_supported\n  - request_object_signing_alg_values_supported\n  - userinfo_signing_alg_values_supported\nnote_on_undeclared:\
  \ >-\n  The discovery document is minimal (541 bytes, Last-Modified 2023-08-17). None\n  of the above OIDC Discovery 1.0 optional members are present, so the scope\n  catalogue, client-authentication methods and claim set cannot be derived from\n  public metadata. They are documented only in the gated integration manual.\n  For this reason no scopes/ artifact is emitted — an OAuthScopes file here\n  would be empty or invented.\nciba:\n  supported: false\n  evidence: >-\n    No backchannel_authentication_endpoint and no\n    urn:openid:params:grant-type:ciba in the discovery document. CAMARA\n    specifies OIDC + CIBA for network-based authorization; DOCOMO advertises\n    neither.\nidentity_assurance:\n  line_authentication: >-\n    DOCOMO documents network line authentication (ネットワーク暗証番号 / 回線認証) and\n    device biometrics behind d ACCOUNT, but these are authentication factors\n    inside the OP, not options a relying party selects through published\n    metadata.\nonboarding:\n  self_serve:\
  \ false\n  steps:\n    - step: 1\n      action: Create a d ACCOUNT (business applicant identity)\n      url: https://id.smt.docomo.ne.jp/cgi8/id/register\n    - step: 2\n      action: >-\n        Register company and applicant information on the d ACCOUNT Connect\n        application site; DOCOMO reviews and replies by email (~3 business days)\n      url: https://g.daccount.docomo.ne.jp/VIEW_OC01/login4\n    - step: 3\n      action: >-\n        Download the integration manual, technical specification and support\n        libraries (available only after approval)\n    - step: 4\n      action: >-\n        Register service and relying-party site configuration; connection is\n        enabled after approval (~3 business days)\n    - step: 5\n      action: Implement d ACCOUNT Connect in the relying-party service\n    - step: 6\n      action: Go live\n  tiers:\n    - tier: Login only (ログイン機能のみ)\n      attributes_released: [user identifier]\n      conditions: none\n      fees: No registration\
  \ fee, no annual fee\n      review: Application required\n    - tier: Login + user information (ログイン機能 + ユーザー情報)\n      attributes_released: [user identifier, email address, customer information]\n      conditions: Third-party certification (第三者認証の取得) required\n      fees: >-\n        Email address is provided free. Other attributes (name, date of birth,\n        etc.) are provided for a fee. Registration/annual fee applies, waived\n        for d POINT / d払い member merchants.\n      review: DOCOMO review (審査) required; contact DOCOMO\n  contact: https://id.smt.docomo.ne.jp/src/dlogin/ctop_method_form.html\nother_transports:\n  - name: docomo Mail IMAP interface\n    auth: >-\n      IMAP over TLS with docomo Mail credentials, specified in the public\n      96-page Japanese PDF (mail_imap_spec_260126.pdf). Not an HTTP API and no\n      token issuance.\n    docs: https://www.docomo.ne.jp/service/developer/smart_phone/application/imap/\nabsent:\n  api_keys: >-\n    No self-serve API key issuance\
  \ exists on any NTT DOCOMO, Inc. host. The\n    first-party \"docomo Developer support\" programme that issued keys closed\n    31 March 2021 and its host no longer resolves.\n  mutual_tls: Not advertised.\n  camara_credentials: >-\n    No CAMARA / GSMA Open Gateway client-credential path is published by\n    DOCOMO. Its announced route (Aduna, partnership concluded 29 January 2026)\n    would issue credentials on the aggregator side, and DOCOMO was not yet\n    listed on Aduna's operator wall as of 2026-07-25.\ncross_reference:\n  well_known: well-known/ntt-docomo-well-known.yml\n  conformance: conformance/ntt-docomo-conformance.yml\n  conventions: conventions/ntt-docomo-conventions.yml\n  domain_security: security/ntt-docomo-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntt-docomo/refs/heads/main/authentication/ntt-docomo-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Telecommunications
- Japan
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Aduna
- Carrier Identity
- SIM Swap
- Number Verification
- Carrier Billing
- 5G
- Partner Gated
---
