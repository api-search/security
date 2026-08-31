---
api_key_in: []
api_specs:
- filename: ustc-campus-status-api-openapi.yml
  format: yaml
  label: USTC Campus Enrollment Status Query API (在校状态查询接口)
  slug: campus-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ustc/refs/heads/main/openapi/ustc-campus-status-api-openapi.yml
auth_types: []
description: 'Authentication posture across every University of Science and Technology of China surface reachable from the open internet. The headline result is that USTC''s identity layer is the institution''s real programmable footprint: USTC''s Network Information Center operates its own CAS/OAuth 2.0/OIDC authorization server at id.ustc.edu.cn, publishes a first-party developer manual for it, serves an anonymously readable OpenID Connect discovery document and JWKS, and runs a separate Shibboleth 5.2.2 identity provider at idp.ustc.edu.cn for federated access. Everything that carries data behind that layer — the enrollment status API, the course catalog, the library OPAC, the campus AI assistant — is gated, and USTC states plainly that relying parties outside the ustc.edu.cn domain are not supported at all.'
kind: authentication
layout: security
method: probed
name: Ustc Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Science and Technology of China declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: University of Science and Technology of China
provider_slug: ustc
scheme_count: 7
schemes:
- authorization_endpoint: https://id.ustc.edu.cn/cas/oidc/authorize
  discovery: https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration
  end_session_endpoint: https://id.ustc.edu.cn/cas/logout
  grant_types:
  - authorization_code
  - password
  - client_credentials
  - refresh_token
  introspection_auth_methods:
  - client_secret_basic
  introspection_endpoint: https://id.ustc.edu.cn/cas/oidc/introspect
  issuer: https://id.ustc.edu.cn/cas
  jwks_uri: https://id.ustc.edu.cn/cas/oidc/jwks
  name: USTC Unified Identity Authentication (OpenID Connect 1.0)
  onboarding: Relying parties are registered by hand. A web application must first complete site registration and filing on USTC's network security platform, then its owner files a 统一身份认证接入申请 (SSO integration request); WeChat official accounts, mini-programs and mobile apps are onboarded by emailing wf0229@ustc.edu.cn. The administrator then issues client_id and client_secret. USTC states explicitly that off-campus applications — those not deployed on campus and not on a ustc.edu.cn domain — are NOT supported ("校外应用（不在校内部署、域名不为 ustc.edu.cn）目前不提供对接支持").
  pkce_advertised: false
  registration_endpoint: https://id.ustc.edu.cn/cas/oidc/register
  registration_endpoint_advertised: true
  registration_endpoint_reachable: false
  response_types:
  - code
  - token
  - id_token token
  revocation_endpoint: https://id.ustc.edu.cn/cas/oidc/revoke
  scopes:
  - openid
  - profile
  - email
  - address
  - phone
  - offline_access
  self_service: false
  software: Ruijie RG-SourceID, CAS-compatible (锐捷 RG-SourceID)
  subject_types:
  - public
  - pairwise
  token_endpoint: https://id.ustc.edu.cn/cas/oidc/accessToken
  token_signing_algorithms:
  - none
  - RS256
  type: openIdConnect
  userinfo_endpoint: https://id.ustc.edu.cn/cas/oidc/profile
  x-operator: institution
- authorization_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/authorize
  detail: The protocol USTC recommends for all new integrations. The developer manual documents the full three-legged exchange with parameter tables, an 8-hour access_token lifetime, and an explicit CSRF warning directing integrators to pass and verify `state`. USTC notes that scope is usually not passed because, for CAS compatibility, attribute release is configured per registered application rather than requested per call.
  documentation: https://id.ustc.edu.cn/doc/developer/
  documented_scopes:
  - gid
  - email
  - name
  evidence: GET /cas/oauth2.0/profile without a token returns 401 {"error":["missing_accessToken"]}
  flow: authorization_code
  name: USTC Unified Identity Authentication (OAuth 2.0 authorization code)
  token_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/accessToken
  token_lifetime_seconds: 28800
  token_type: bearer
  type: oauth2
  userinfo_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/profile
  x-operator: institution
- detail: Retained as a compatibility protocol; USTC recommends OAuth 2.0 for new applications. The CAS ticket validation endpoint answers unauthenticated callers with a well-formed cas:serviceResponse envelope, which is how the protocol was confirmed rather than assumed.
  evidence: GET https://passport.ustc.edu.cn/serviceValidate returns 200 text/plain with <cas:serviceResponse …><cas:authenticationFailure code="INTERNAL_ERROR">ticket或service参数为空
  login_endpoint: https://id.ustc.edu.cn/cas/login
  name: USTC Unified Identity Authentication (CAS 3.0)
  protocol: https://apereo.github.io/cas/development/protocol/CAS-Protocol-Specification.html
  type: cas
  validate_endpoint: https://passport.ustc.edu.cn/serviceValidate
  x-operator: institution
- detail: See identity-federation/ustc-identity-federation.yml
  entityID: https://idp.ustc.edu.cn/idp/shibboleth
  federations:
  - CARSI (中国教育科研计算机网统一认证与资源共享基础设施)
  - CSTCloud AAI (中国科学院科技云认证和授权基础设施)
  - eduGAIN
  metadata: https://idp.ustc.edu.cn/idp/shibboleth
  name: Shibboleth / SAML 2.0 identity provider
  scope: ustc.edu.cn
  software: Shibboleth IdP 5.2.2
  type: saml2
  x-operator: institution
- applies_to: https://id.ustc.edu.cn/doc/api/
  detail: The enrollment status API requires both a bearer token issued by the administrator and a source IP registered in an allowlist; either alone is refused, with 401 and 403 documented as distinct outcomes. Onboarding requires a system name, a fixed egress IP or range, and a named contact. There is no self-service path.
  evidence: 401 {"detail":"missing or invalid bearer token"} observed 2026-08-30
  name: Administrator-issued bearer token plus source-IP allowlist
  scheme: bearer
  type: http
  x-additional-control: source IP allowlist
  x-operator: institution
- applies_to:
  - https://catalog.ustc.edu.cn/api/teach/
  - https://opac.lib.ustc.edu.cn/
  - https://chat.ustc.edu.cn/
  detail: The course catalog's JSON API, the library OPAC and the campus AI assistant are all real institution-operated surfaces behind the unified identity session. None publishes an authentication contract of its own. The catalog is additionally in a declared restricted mode, and the OPAC refuses off-campus source IPs in prose before any credential is offered.
  evidence: GET https://catalog.ustc.edu.cn/api/teach/semester/list -> 401 (empty body); GET https://catalog.ustc.edu.cn/api/restricted -> 200 {"restricted":true}; GET https://opac.lib.ustc.edu.cn/ -> 200 with "您从校外 (…) 访问 …，需要先验证身份才允许继续访问"
  in: cookie
  name: Session cookie behind unified identity (undocumented)
  type: apiKey
  x-operator: institution
- applies_to:
  - https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration
  - https://id.ustc.edu.cn/cas/oidc/jwks
  - https://id.ustc.edu.cn/doc/api/health
  - https://passport.ustc.edu.cn/healthcheck
  - https://idp.ustc.edu.cn/idp/shibboleth
  - https://mirrors.ustc.edu.cn/
  detail: What USTC does publish openly is protocol metadata, two health checks and a package mirror. All six are institution-operated — mirrors.ustc.edu.cn resolves into 202.38.95.110, inside the APNIC block registered to "The University of Science and Technology of China" itself.
  name: Anonymous read
  type: none
  x-operator: institution
slug: ustc-authentication
source_filename: ustc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication Posture\nspecificationVersion: '0.1'\nprovider: University of Science and Technology of China\nproviderId: ustc\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live fetches on 2026-08-30, all with a browser User-Agent:\n  https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration (200, application/json, 1271 bytes),\n  https://id.ustc.edu.cn/cas/oidc/jwks (200, application/json, one RS256 RSA key),\n  https://id.ustc.edu.cn/doc/developer/ (200 — USTC's own developer manual for CAS 3.0 / OAuth 2.0 / OIDC 1.0),\n  https://id.ustc.edu.cn/doc/status-api/ (200 — bearer-token + IP-allowlist scheme for the status API),\n  https://id.ustc.edu.cn/cas/oauth2.0/profile (401, {\"error\":[\"missing_accessToken\"]}),\n  https://id.ustc.edu.cn/doc/api/status/by-zjhm/P0529 (401, {\"detail\":\"missing or invalid bearer token\"}),\n  https://passport.ustc.edu.cn/serviceValidate (200, CAS 2.0 XML authenticationFailure envelope),\n  https://passport.ustc.edu.cn/healthcheck\
  \ (200, text/plain \"OK\"),\n  https://idp.ustc.edu.cn/idp/shibboleth (200, application/xml, 15,066-byte SAML 2.0 EntityDescriptor),\n  https://catalog.ustc.edu.cn/api/teach/semester/list (401),\n  https://catalog.ustc.edu.cn/api/restricted (200, {\"restricted\":true}).\ndescription: >-\n  Authentication posture across every University of Science and Technology of China surface\n  reachable from the open internet. The headline result is that USTC's identity layer is the\n  institution's real programmable footprint: USTC's Network Information Center operates its own\n  CAS/OAuth 2.0/OIDC authorization server at id.ustc.edu.cn, publishes a first-party developer\n  manual for it, serves an anonymously readable OpenID Connect discovery document and JWKS, and\n  runs a separate Shibboleth 5.2.2 identity provider at idp.ustc.edu.cn for federated access.\n  Everything that carries data behind that layer — the enrollment status API, the course\n  catalog, the library OPAC, the campus AI assistant\
  \ — is gated, and USTC states plainly that\n  relying parties outside the ustc.edu.cn domain are not supported at all.\n\nschemes:\n- name: USTC Unified Identity Authentication (OpenID Connect 1.0)\n  type: openIdConnect\n  x-operator: institution\n  issuer: https://id.ustc.edu.cn/cas\n  discovery: https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration\n  jwks_uri: https://id.ustc.edu.cn/cas/oidc/jwks\n  authorization_endpoint: https://id.ustc.edu.cn/cas/oidc/authorize\n  token_endpoint: https://id.ustc.edu.cn/cas/oidc/accessToken\n  userinfo_endpoint: https://id.ustc.edu.cn/cas/oidc/profile\n  introspection_endpoint: https://id.ustc.edu.cn/cas/oidc/introspect\n  revocation_endpoint: https://id.ustc.edu.cn/cas/oidc/revoke\n  registration_endpoint: https://id.ustc.edu.cn/cas/oidc/register\n  end_session_endpoint: https://id.ustc.edu.cn/cas/logout\n  scopes:\n  - openid\n  - profile\n  - email\n  - address\n  - phone\n  - offline_access\n  grant_types:\n  - authorization_code\n\
  \  - password\n  - client_credentials\n  - refresh_token\n  response_types:\n  - code\n  - token\n  - id_token token\n  subject_types:\n  - public\n  - pairwise\n  token_signing_algorithms:\n  - none\n  - RS256\n  introspection_auth_methods:\n  - client_secret_basic\n  pkce_advertised: false\n  registration_endpoint_advertised: true\n  registration_endpoint_reachable: false\n  self_service: false\n  onboarding: >-\n    Relying parties are registered by hand. A web application must first complete site\n    registration and filing on USTC's network security platform, then its owner files a\n    统一身份认证接入申请 (SSO integration request); WeChat official accounts, mini-programs and\n    mobile apps are onboarded by emailing wf0229@ustc.edu.cn. The administrator then issues\n    client_id and client_secret. USTC states explicitly that off-campus applications — those not\n    deployed on campus and not on a ustc.edu.cn domain — are NOT supported\n    (\"校外应用（不在校内部署、域名不为 ustc.edu.cn）目前不提供对接支持\").\n\
  \  software: Ruijie RG-SourceID, CAS-compatible (锐捷 RG-SourceID)\n- name: USTC Unified Identity Authentication (OAuth 2.0 authorization code)\n  type: oauth2\n  x-operator: institution\n  flow: authorization_code\n  authorization_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/authorize\n  token_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/accessToken\n  userinfo_endpoint: https://id.ustc.edu.cn/cas/oauth2.0/profile\n  token_type: bearer\n  token_lifetime_seconds: 28800\n  documented_scopes:\n  - gid\n  - email\n  - name\n  documentation: https://id.ustc.edu.cn/doc/developer/\n  detail: >-\n    The protocol USTC recommends for all new integrations. The developer manual documents the\n    full three-legged exchange with parameter tables, an 8-hour access_token lifetime, and an\n    explicit CSRF warning directing integrators to pass and verify `state`. USTC notes that\n    scope is usually not passed because, for CAS compatibility, attribute release is configured\n    per registered application\
  \ rather than requested per call.\n  evidence: 'GET /cas/oauth2.0/profile without a token returns 401 {\"error\":[\"missing_accessToken\"]}'\n- name: USTC Unified Identity Authentication (CAS 3.0)\n  type: cas\n  x-operator: institution\n  protocol: https://apereo.github.io/cas/development/protocol/CAS-Protocol-Specification.html\n  login_endpoint: https://id.ustc.edu.cn/cas/login\n  validate_endpoint: https://passport.ustc.edu.cn/serviceValidate\n  detail: >-\n    Retained as a compatibility protocol; USTC recommends OAuth 2.0 for new applications. The\n    CAS ticket validation endpoint answers unauthenticated callers with a well-formed\n    cas:serviceResponse envelope, which is how the protocol was confirmed rather than assumed.\n  evidence: >-\n    GET https://passport.ustc.edu.cn/serviceValidate returns 200 text/plain with\n    <cas:serviceResponse …><cas:authenticationFailure code=\"INTERNAL_ERROR\">ticket或service参数为空\n- name: Shibboleth / SAML 2.0 identity provider\n  type: saml2\n\
  \  x-operator: institution\n  entityID: https://idp.ustc.edu.cn/idp/shibboleth\n  metadata: https://idp.ustc.edu.cn/idp/shibboleth\n  scope: ustc.edu.cn\n  software: Shibboleth IdP 5.2.2\n  federations:\n  - CARSI (中国教育科研计算机网统一认证与资源共享基础设施)\n  - CSTCloud AAI (中国科学院科技云认证和授权基础设施)\n  - eduGAIN\n  detail: See identity-federation/ustc-identity-federation.yml\n- name: Administrator-issued bearer token plus source-IP allowlist\n  type: http\n  scheme: bearer\n  x-operator: institution\n  applies_to: https://id.ustc.edu.cn/doc/api/\n  x-additional-control: source IP allowlist\n  detail: >-\n    The enrollment status API requires both a bearer token issued by the administrator and a\n    source IP registered in an allowlist; either alone is refused, with 401 and 403 documented\n    as distinct outcomes. Onboarding requires a system name, a fixed egress IP or range, and a\n    named contact. There is no self-service path.\n  evidence: '401 {\"detail\":\"missing or invalid bearer token\"} observed\
  \ 2026-08-30'\n- name: Session cookie behind unified identity (undocumented)\n  type: apiKey\n  in: cookie\n  x-operator: institution\n  applies_to:\n  - https://catalog.ustc.edu.cn/api/teach/\n  - https://opac.lib.ustc.edu.cn/\n  - https://chat.ustc.edu.cn/\n  detail: >-\n    The course catalog's JSON API, the library OPAC and the campus AI assistant are all real\n    institution-operated surfaces behind the unified identity session. None publishes an\n    authentication contract of its own. The catalog is additionally in a declared restricted\n    mode, and the OPAC refuses off-campus source IPs in prose before any credential is offered.\n  evidence: >-\n    GET https://catalog.ustc.edu.cn/api/teach/semester/list -> 401 (empty body);\n    GET https://catalog.ustc.edu.cn/api/restricted -> 200 {\"restricted\":true};\n    GET https://opac.lib.ustc.edu.cn/ -> 200 with \"您从校外 (…) 访问 …，需要先验证身份才允许继续访问\"\n- name: Anonymous read\n  type: none\n  x-operator: institution\n  applies_to:\n  - https://id.ustc.edu.cn/cas/oidc/.well-known/openid-configuration\n\
  \  - https://id.ustc.edu.cn/cas/oidc/jwks\n  - https://id.ustc.edu.cn/doc/api/health\n  - https://passport.ustc.edu.cn/healthcheck\n  - https://idp.ustc.edu.cn/idp/shibboleth\n  - https://mirrors.ustc.edu.cn/\n  detail: >-\n    What USTC does publish openly is protocol metadata, two health checks and a package mirror.\n    All six are institution-operated — mirrors.ustc.edu.cn resolves into 202.38.95.110, inside\n    the APNIC block registered to \"The University of Science and Technology of China\" itself.\n\nobservations:\n- >-\n  USTC advertises the `password` and `client_credentials` grant types and the `token` and\n  `id_token token` response types in its live OIDC discovery document. The implicit-style\n  response types and the resource-owner password grant are both deprecated by OAuth 2.1 and the\n  IETF security BCP. This is what the institution's discovery document currently tells clients\n  is available.\n- >-\n  `id_token_signing_alg_values_supported` includes `none` alongside\
  \ RS256. An unsigned ID token\n  is accepted at the protocol level by anything that reads this document literally.\n- >-\n  `code_challenge_methods_supported` is absent, so PKCE cannot be discovered by a conformant\n  client even if the server supports it.\n- >-\n  A `registration_endpoint` is advertised at /cas/oidc/register but returns 404 to an\n  unauthenticated GET. Dynamic client registration is announced in metadata and not actually\n  open — the discovery document overstates what an integrator can do.\n- >-\n  There is no route to a client_id for anyone outside the institution. USTC says so directly\n  rather than leaving it to be discovered, which is more honest than most of this cohort.\n- >-\n  passport.ustc.edu.cn and id.ustc.edu.cn resolve to the same address, 210.45.67.89. passport\n  is the legacy hostname kept alive for redirects since the February 2025 cutover; it still\n  answers the CAS validation and healthcheck paths but 404s the OIDC discovery path, so the two\n \
  \ names are not interchangeable for integrators.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ustc/refs/heads/main/authentication/ustc-authentication.yml
summary_line: 7 schemes
tags:
- University
- Higher Education
- Education
- China
- C9 League
- Chinese Academy of Sciences
- Research
- Identity Federation
- Single Sign-On
- Course Catalog
- Research Computing
- Open Source Mirror
---
