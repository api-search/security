---
api_key_in: []
api_specs:
- filename: iit-bombay-instiapp-api-openapi.yml
  format: yaml
  label: InstiApp API
  slug: instiapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/openapi/iit-bombay-instiapp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Iit Bombay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indian Institute of Technology Bombay declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Indian Institute of Technology Bombay
provider_slug: iit-bombay
scheme_count: 4
schemes:
- authorization_endpoint: https://sso.iitb.ac.in/authorize
  discovery: https://sso.iitb.ac.in/.well-known/openid-configuration
  discovery_status: 200
  flow: authorization_code
  human_factors: Interactive sign-in is LDAP username plus a second factor — TOTP from a registered authenticator app, a hardware credential (WebAuthn/U2F), or an OTP over SMS. This is the credential every institutional service behind asc.iitb.ac.in sits on.
  issuer: https://sso.iitb.ac.in
  jwks_uri: https://sso.iitb.ac.in/.well-known/jwks.json
  name: IITB Central SSO (OpenID Connect)
  note: This is the find of the 2026-08-30 pass. A machine-readable, institution-operated identity discovery document is exactly the surface class the university pipeline says is real and almost never catalogued, and it was absent from this repo entirely.
  operator: institution
  operator_evidence: Host sso.iitb.ac.in is under the institution registrable domain iitb.ac.in; the sign-in page is branded "Computer Center, IIT Bombay"; the discovery document's issuer is https://sso.iitb.ac.in itself, not a vendor's issuer.
  probes:
  - detail: valid JSON discovery document, 381 bytes
    status: 200
    url: https://sso.iitb.ac.in/.well-known/openid-configuration
  - detail: JWKS with one RSA key, kid "sso"
    status: 200
    url: https://sso.iitb.ac.in/.well-known/jwks.json
  - detail: '{"message":"Invalid request: method must be POST","name":"invalid_request"} — endpoint live'
    status: 400
    url: https://sso.iitb.ac.in/token
  - detail: '{"message":"Unauthorized request: no authentication given","name":"unauthorized_request"} — endpoint live'
    status: 401
    url: https://sso.iitb.ac.in/user
  registration: Client registration is not self-service and no public registration endpoint was found. The Gymkhana developer documentation directs external developers to the Computer Centre for IITB SSO integration.
  response_types_supported:
  - code
  scopes_supported:
  - openid
  standard: OpenID Connect Discovery 1.0
  token_endpoint: https://sso.iitb.ac.in/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: oauth2
  userinfo_endpoint: https://sso.iitb.ac.in/user
- authorization_endpoint: https://gymkhana.iitb.ac.in/profiles/oauth/authorize/
  client_types:
  - confidential
  - public
  discovery: null
  discovery_note: No RFC 8414 authorization-server metadata is published; /profiles/.well-known/openid-configuration returns 404. Endpoints are documented in prose only.
  eligibility_restriction: The documentation states plainly that Profiles is intended ONLY for applications running on IIT Bombay Students' Gymkhana server infrastructure, and that applications which do not may be deleted and the account blocked without notice. This is a real access boundary, not a formality — it is why this surface is documented-but-not-open.
  flow: authorization_code
  name: Gymkhana Profiles (OAuth 2.0)
  operator: institution
  operator_evidence: Host gymkhana.iitb.ac.in is under iitb.ac.in; the implementation is published by the institution's own student body at github.com/iitb-gymkhana/sso (GPL-3.0), whose declared homepage is this endpoint.
  probes:
  - status: 200
    url: https://gymkhana.iitb.ac.in/profiles/doc/
  - status: 200
    url: https://gymkhana.iitb.ac.in/profiles/oauth/authorize/
  - detail: Method Not Allowed on GET — POST-only token endpoint, live
    status: 405
    url: https://gymkhana.iitb.ac.in/profiles/oauth/token/
  - detail: '{"detail":"Authentication credentials were not provided."} — live protected resource'
    status: 401
    url: https://gymkhana.iitb.ac.in/profiles/user/api/user/
  - status: 404
    url: https://gymkhana.iitb.ac.in/profiles/.well-known/openid-configuration
  resource_endpoint: https://gymkhana.iitb.ac.in/profiles/user/api/user/
  scopes: scopes/iit-bombay-scopes.yml
  standard: RFC 6749
  token_endpoint: https://gymkhana.iitb.ac.in/profiles/oauth/token/
  type: oauth2
- actual_behaviour: The declared HTTP Basic scheme is what drf-yasg emitted; in practice the deployed API serves a substantial read-only surface with NO credential at all, and gates the rest behind a session established via the /login flow (which itself brokers Gymkhana SSO). This mismatch between the declared scheme and the deployed behaviour is recorded, not corrected — the institution's own document is the source.
  authenticated_only_confirmed:
  - path: /user-me
    status: 401
  - path: /achievements
    status: 401
  - path: /placement-blog
    status: 401
  - path: /training-blog
    status: 401
  - path: /query
    status: 401
  - path: /calendar/feed/
    status: 403
  declared_in_spec:
    securitySchemes:
      Basic:
        scheme: basic
        type: http
    security_applied_globally: true
  login_flow: https://gymkhana.iitb.ac.in/instiapp/api/login
  name: InstiApp API
  operator: institution
  operator_evidence: servers[0].url is https://gymkhana.iitb.ac.in/instiapp/api; info.contact.email is devcom@iitb.ac.in; source at github.com/DevCom-IITB/instiapp-api (AGPL-3.0).
  type: mixed
  unauthenticated_read_confirmed:
  - path: /events
    status: 200
  - path: /bodies
    status: 200
  - path: /news
    status: 200
  - path: /mess
    status: 200
  - path: /locations
    status: 200
  - path: /search
    status: 200
  - path: /buy/products
    status: 200
  - path: /venter/complaints
    status: 200
  - path: /venter/tags
    status: 200
- authorization_endpoint: https://sso.tech-iitb.org/ssocall
  discovery: null
  exchange_endpoint: https://sso.tech-iitb.org/getuserdata
  flow: redirect + server-side exchange
  name: ITC Single Sign-On
  operator: tenant
  operator_evidence: Operated by the Institute Technical Council, an IIT Bombay student body, but NOT on an institution-owned host. tech-iitb.org was registered 2024-10-02 through Hostinger and resolves to 82.112.236.232 (Hostinger). The institution's own registrable domain is iitb.ac.in. Under the university pipeline's operator axis this is a student-body surface on a non-institution domain — a real relationship, recorded as tenant rather than credited to the institution's engineering.
  probes:
  - status: 200
    url: https://sso.tech-iitb.org/docs/
  - status: 404
    url: https://sso.tech-iitb.org/.well-known/openid-configuration
  session_ttl: 1 hour (per published documentation)
  standard: none declared
  type: session
slug: iit-bombay-authentication
source_filename: iit-bombay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://gymkhana.iitb.ac.in/instiapp/api/docs/?format=openapi\ndocs: https://gymkhana.iitb.ac.in/profiles/doc/\nnote: >-\n  IIT Bombay runs three distinct, independently-operated authentication surfaces, and telling\n  them apart is the whole point of this file. Two are on the institution's own registrable\n  domain (iitb.ac.in) and one is not. Every scheme below was probed live on 2026-08-30; status\n  codes are recorded rather than inferred from documentation.\nx-operator-summary:\n  institution:\n  - https://sso.iitb.ac.in\n  - https://gymkhana.iitb.ac.in/profiles/\n  - https://gymkhana.iitb.ac.in/instiapp/api\n  tenant:\n  - https://sso.tech-iitb.org/\nschemes:\n\n- name: IITB Central SSO (OpenID Connect)\n  operator: institution\n  operator_evidence: >-\n    Host sso.iitb.ac.in is under the institution registrable domain iitb.ac.in; the sign-in page\n    is branded \"Computer Center, IIT Bombay\"; the discovery document's\
  \ issuer is\n    https://sso.iitb.ac.in itself, not a vendor's issuer.\n  type: oauth2\n  flow: authorization_code\n  standard: OpenID Connect Discovery 1.0\n  discovery: https://sso.iitb.ac.in/.well-known/openid-configuration\n  discovery_status: 200\n  issuer: https://sso.iitb.ac.in\n  authorization_endpoint: https://sso.iitb.ac.in/authorize\n  token_endpoint: https://sso.iitb.ac.in/token\n  userinfo_endpoint: https://sso.iitb.ac.in/user\n  jwks_uri: https://sso.iitb.ac.in/.well-known/jwks.json\n  scopes_supported: [ openid ]\n  response_types_supported: [ code ]\n  token_endpoint_auth_methods_supported: [ client_secret_basic ]\n  probes:\n  - url: https://sso.iitb.ac.in/.well-known/openid-configuration\n    status: 200\n    detail: valid JSON discovery document, 381 bytes\n  - url: https://sso.iitb.ac.in/.well-known/jwks.json\n    status: 200\n    detail: 'JWKS with one RSA key, kid \"sso\"'\n  - url: https://sso.iitb.ac.in/token\n    status: 400\n    detail: '{\"message\":\"Invalid\
  \ request: method must be POST\",\"name\":\"invalid_request\"} — endpoint live'\n  - url: https://sso.iitb.ac.in/user\n    status: 401\n    detail: '{\"message\":\"Unauthorized request: no authentication given\",\"name\":\"unauthorized_request\"} — endpoint live'\n  human_factors: >-\n    Interactive sign-in is LDAP username plus a second factor — TOTP from a registered\n    authenticator app, a hardware credential (WebAuthn/U2F), or an OTP over SMS. This is the\n    credential every institutional service behind asc.iitb.ac.in sits on.\n  registration: >-\n    Client registration is not self-service and no public registration endpoint was found. The\n    Gymkhana developer documentation directs external developers to the Computer Centre for\n    IITB SSO integration.\n  note: >-\n    This is the find of the 2026-08-30 pass. A machine-readable, institution-operated identity\n    discovery document is exactly the surface class the university pipeline says is real and\n    almost never catalogued,\
  \ and it was absent from this repo entirely.\n\n- name: Gymkhana Profiles (OAuth 2.0)\n  operator: institution\n  operator_evidence: >-\n    Host gymkhana.iitb.ac.in is under iitb.ac.in; the implementation is published by the\n    institution's own student body at github.com/iitb-gymkhana/sso (GPL-3.0), whose declared\n    homepage is this endpoint.\n  type: oauth2\n  flow: authorization_code\n  standard: RFC 6749\n  authorization_endpoint: https://gymkhana.iitb.ac.in/profiles/oauth/authorize/\n  token_endpoint: https://gymkhana.iitb.ac.in/profiles/oauth/token/\n  resource_endpoint: https://gymkhana.iitb.ac.in/profiles/user/api/user/\n  discovery: null\n  discovery_note: >-\n    No RFC 8414 authorization-server metadata is published;\n    /profiles/.well-known/openid-configuration returns 404. Endpoints are documented in prose\n    only.\n  client_types: [ confidential, public ]\n  scopes: scopes/iit-bombay-scopes.yml\n  probes:\n  - url: https://gymkhana.iitb.ac.in/profiles/doc/\n   \
  \ status: 200\n  - url: https://gymkhana.iitb.ac.in/profiles/oauth/authorize/\n    status: 200\n  - url: https://gymkhana.iitb.ac.in/profiles/oauth/token/\n    status: 405\n    detail: Method Not Allowed on GET — POST-only token endpoint, live\n  - url: https://gymkhana.iitb.ac.in/profiles/user/api/user/\n    status: 401\n    detail: '{\"detail\":\"Authentication credentials were not provided.\"} — live protected resource'\n  - url: https://gymkhana.iitb.ac.in/profiles/.well-known/openid-configuration\n    status: 404\n  eligibility_restriction: >-\n    The documentation states plainly that Profiles is intended ONLY for applications running on\n    IIT Bombay Students' Gymkhana server infrastructure, and that applications which do not\n    may be deleted and the account blocked without notice. This is a real access boundary, not\n    a formality — it is why this surface is documented-but-not-open.\n\n- name: InstiApp API\n  operator: institution\n  operator_evidence: >-\n    servers[0].url\
  \ is https://gymkhana.iitb.ac.in/instiapp/api; info.contact.email is\n    devcom@iitb.ac.in; source at github.com/DevCom-IITB/instiapp-api (AGPL-3.0).\n  type: mixed\n  declared_in_spec:\n    securitySchemes:\n      Basic:\n        type: http\n        scheme: basic\n    security_applied_globally: true\n  actual_behaviour: >-\n    The declared HTTP Basic scheme is what drf-yasg emitted; in practice the deployed API serves\n    a substantial read-only surface with NO credential at all, and gates the rest behind a\n    session established via the /login flow (which itself brokers Gymkhana SSO). This mismatch\n    between the declared scheme and the deployed behaviour is recorded, not corrected — the\n    institution's own document is the source.\n  unauthenticated_read_confirmed:\n  - { path: /events, status: 200 }\n  - { path: /bodies, status: 200 }\n  - { path: /news, status: 200 }\n  - { path: /mess, status: 200 }\n  - { path: /locations, status: 200 }\n  - { path: /search, status: 200\
  \ }\n  - { path: /buy/products, status: 200 }\n  - { path: /venter/complaints, status: 200 }\n  - { path: /venter/tags, status: 200 }\n  authenticated_only_confirmed:\n  - { path: /user-me, status: 401 }\n  - { path: /achievements, status: 401 }\n  - { path: /placement-blog, status: 401 }\n  - { path: /training-blog, status: 401 }\n  - { path: /query, status: 401 }\n  - { path: /calendar/feed/, status: 403 }\n  login_flow: https://gymkhana.iitb.ac.in/instiapp/api/login\n\n- name: ITC Single Sign-On\n  operator: tenant\n  operator_evidence: >-\n    Operated by the Institute Technical Council, an IIT Bombay student body, but NOT on an\n    institution-owned host. tech-iitb.org was registered 2024-10-02 through Hostinger and\n    resolves to 82.112.236.232 (Hostinger). The institution's own registrable domain is\n    iitb.ac.in. Under the university pipeline's operator axis this is a student-body surface on\n    a non-institution domain — a real relationship, recorded as tenant rather than\
  \ credited to\n    the institution's engineering.\n  type: session\n  flow: redirect + server-side exchange\n  standard: none declared\n  authorization_endpoint: https://sso.tech-iitb.org/ssocall\n  exchange_endpoint: https://sso.tech-iitb.org/getuserdata\n  discovery: null\n  probes:\n  - url: https://sso.tech-iitb.org/docs/\n    status: 200\n  - url: https://sso.tech-iitb.org/.well-known/openid-configuration\n    status: 404\n  session_ttl: 1 hour (per published documentation)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/authentication/iit-bombay-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- India
- Institute of Technology
- Research
- Identity
- Single Sign-On
- OpenID Connect
- Campus Life
- Research Repository
- Open Source
---
