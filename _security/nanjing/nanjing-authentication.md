---
api_key_in: []
auth_types:
- none
- saml
- cas
- bearer
- challenge
description: ''
kind: authentication
layout: security
method: probed
name: Nanjing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nanjing University secures its APIs with none, saml, cas, bearer, and challenge across 9 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nanjing University
provider_slug: nanjing
scheme_count: 9
schemes:
- applies_to: https://mirrors.nju.edu.cn/configs
  description: 'NJU Mirror''s JSON configuration endpoints are open, unauthenticated reads and answer application/json. One quirk worth recording: the site''s edge sets a `bcheck=true` cookie and 302s a first-time client back to itself; sending that cookie makes every route answer normally. It is a cookie check, not an authentication scheme.'
  evidence:
    status: 200
    url: https://mirrors.nju.edu.cn/configs/documentations/index.json
  name: MirrorConfigPublic
  operator: institution
  type: none
- applies_to: https://box.nju.edu.cn/api2
  description: NJU Box (南大云盘) answers /api2/ping/ and /api2/server-info/ to an anonymous caller. Everything beyond service discovery requires an NJU account token.
  evidence:
    status: 200
    url: https://box.nju.edu.cn/api2/server-info/
  name: SeafileServerInfoPublic
  operator: institution
  type: none
- applies_to: https://table.nju.edu.cn
  description: NJU Table (南大表格) answers /api2/ping/ and /server-info/ anonymously; the SeaTable API beyond that requires an account token.
  evidence:
    status: 200
    url: https://table.nju.edu.cn/server-info/
  name: SeaTableServerInfoPublic
  operator: institution
  type: none
- applies_to: https://pass.nju.edu.cn
  description: NJU's password manager exposes /alive and /api/config unauthenticated (server identity, version, vault and API base URLs). The vault API itself is Bitwarden-protocol and requires account credentials.
  evidence:
    status: 200
    url: https://pass.nju.edu.cn/api/config
  name: VaultwardenStatusPublic
  operator: institution
  type: none
- additional_evidence:
  - status: 200
    url: https://authserver.nju.edu.cn/authserver/login
  - note: Probed for an OIDC discovery document; the CAS server returns a JSON 404 ({"error":"Not Found"}). No OpenID Connect surface is published.
    status: 404
    url: https://authserver.nju.edu.cn/authserver/.well-known/openid-configuration
  applies_to: https://authserver.nju.edu.cn/authserver/
  description: 'Nanjing University''s central single sign-on is a CAS deployment. Ticket validation is publicly reachable and speaks the protocol to an anonymous caller: /authserver/serviceValidate (CAS 2.0) and /authserver/p3/serviceValidate (CAS 3.0) both return application/xml <cas:serviceResponse> with <cas:authenticationFailure code="INVALID_TICKET">. Login supports password, verification code, biometric and QR-code methods. There is no public service registration: a relying service must be registered by NJU IT, so third parties cannot obtain a CAS client.'
  evidence:
    status: 200
    url: https://authserver.nju.edu.cn/authserver/p3/serviceValidate?service=https%3A%2F%2Fexample.org%2F&ticket=ST-test
  name: CasSingleSignOn
  operator: institution
  type: cas
- additional_evidence:
  - note: correct protocol rejection of a request carrying no SAMLRequest
    status: 400
    url: https://idp.nju.edu.cn/idp/profile/SAML2/Redirect/SSO
  applies_to: https://idp.nju.edu.cn/idp/shibboleth
  description: SAML 2.0 web SSO through NJU's own Shibboleth IdP, registered in CARSI and republished to eduGAIN. Used in production by the university library for off-campus access to licensed resources. Metadata is public; assertions require an NJU account.
  evidence:
    status: 200
    url: https://idp.nju.edu.cn/idp/shibboleth
  name: ShibbolethSaml
  operator: institution
  type: saml
- additional_evidence:
  - note: public HTML API reference
    status: 200
    url: https://doc.nju.edu.cn/api/docs
  - note: the JSON description of the API requires the token the API requires
    status: 401
    url: https://doc.nju.edu.cn/api/docs.json
  applies_to: https://doc.nju.edu.cn/api
  description: 'The e-Science Document service publishes complete REST API documentation publicly at /api/docs — 79 endpoints across books, chapters, pages, shelves, attachments, images, users, roles, recycle-bin, audit-log and search, with GET/POST/PUT/DELETE. The API itself is token-gated: an unauthenticated call returns a clean JSON error envelope, {"error":{"message":"No authorization token found on the request","code":401}}. Tokens are issued to NJU account holders from the user profile; there is no public registration. The machine-readable description at /api/docs.json is itself behind the token, so the only public description of this API is the HTML page.'
  evidence:
    status: 401
    url: https://doc.nju.edu.cn/api/books
  name: BookStackApiToken
  operator: institution
  type: bearer
- applies_to: https://git.nju.edu.cn/api/v4
  description: NJU's GitLab instance sits behind an Anubis proof-of-work bot challenge. Every /api/v4 route answers HTTP 200 with the challenge page ("Making sure you're not a bot!") to a non-browser client, so the API is live and gated rather than dead or absent — the university's own mirror site calls https://git.nju.edu.cn/api/v4/projects/2412/issues from a browser to render its announcements. This is an anti-crawler control, not an authorization scheme; it is recorded here because it is what a client encounters first.
  evidence:
    note: 200 body is the Anubis challenge, not the resource
    status: 200
    url: https://git.nju.edu.cn/api/v4/projects/2412/issues
  name: AnubisBotChallenge
  operator: institution
  type: challenge
- applies_to: https://opac.nju.edu.cn
  description: 'The library OPAC is restricted to the campus network: every route, including /oai?verb=Identify, returns HTTP 403 with the body "请使用南大VPN访问!" ("please access via the NJU VPN"). Live and gated by network location, not credentials.'
  evidence:
    status: 403
    url: https://opac.nju.edu.cn/
  name: CampusNetworkGate
  operator: institution
  type: challenge
slug: nanjing-authentication
source_filename: nanjing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of every surface attributed to Nanjing University in this profile.\n  Each scheme below names the exact URL that demonstrated it. Nothing here is inferred from a\n  vendor's generic documentation: where the software is a third party's, the scheme recorded is\n  the one NJU's own deployment actually answered with.\nprovider: Nanjing University\nproviderId: nanjing\nsummary:\n  types:\n    - none\n    - saml\n    - cas\n    - bearer\n    - challenge\n  institution_operated_public_surfaces_requiring_no_auth: 4\n  note: >-\n    Nanjing University operates no API key programme, no OAuth client registration, no developer\n    portal and no published API terms of service. Every authenticated surface below is gated on an\n    NJU institutional account, and the credentials are issued through central IT (ITSC), not\n    self-service. There is nothing here a member of the public can sign up for.\nschemes:\n\
  \  - name: MirrorConfigPublic\n    type: none\n    operator: institution\n    applies_to: https://mirrors.nju.edu.cn/configs\n    description: >-\n      NJU Mirror's JSON configuration endpoints are open, unauthenticated reads and answer\n      application/json. One quirk worth recording: the site's edge sets a `bcheck=true` cookie and\n      302s a first-time client back to itself; sending that cookie makes every route answer\n      normally. It is a cookie check, not an authentication scheme.\n    evidence:\n      url: https://mirrors.nju.edu.cn/configs/documentations/index.json\n      status: 200\n  - name: SeafileServerInfoPublic\n    type: none\n    operator: institution\n    applies_to: https://box.nju.edu.cn/api2\n    description: >-\n      NJU Box (南大云盘) answers /api2/ping/ and /api2/server-info/ to an anonymous caller. Everything\n      beyond service discovery requires an NJU account token.\n    evidence:\n      url: https://box.nju.edu.cn/api2/server-info/\n      status: 200\n\
  \  - name: SeaTableServerInfoPublic\n    type: none\n    operator: institution\n    applies_to: https://table.nju.edu.cn\n    description: >-\n      NJU Table (南大表格) answers /api2/ping/ and /server-info/ anonymously; the SeaTable API beyond\n      that requires an account token.\n    evidence:\n      url: https://table.nju.edu.cn/server-info/\n      status: 200\n  - name: VaultwardenStatusPublic\n    type: none\n    operator: institution\n    applies_to: https://pass.nju.edu.cn\n    description: >-\n      NJU's password manager exposes /alive and /api/config unauthenticated (server identity,\n      version, vault and API base URLs). The vault API itself is Bitwarden-protocol and requires\n      account credentials.\n    evidence:\n      url: https://pass.nju.edu.cn/api/config\n      status: 200\n  - name: CasSingleSignOn\n    type: cas\n    operator: institution\n    applies_to: https://authserver.nju.edu.cn/authserver/\n    description: >-\n      Nanjing University's central single sign-on\
  \ is a CAS deployment. Ticket validation is\n      publicly reachable and speaks the protocol to an anonymous caller: /authserver/serviceValidate\n      (CAS 2.0) and /authserver/p3/serviceValidate (CAS 3.0) both return\n      application/xml <cas:serviceResponse> with <cas:authenticationFailure code=\"INVALID_TICKET\">.\n      Login supports password, verification code, biometric and QR-code methods. There is no public\n      service registration: a relying service must be registered by NJU IT, so third parties cannot\n      obtain a CAS client.\n    evidence:\n      url: https://authserver.nju.edu.cn/authserver/p3/serviceValidate?service=https%3A%2F%2Fexample.org%2F&ticket=ST-test\n      status: 200\n    additional_evidence:\n      - url: https://authserver.nju.edu.cn/authserver/login\n        status: 200\n      - url: https://authserver.nju.edu.cn/authserver/.well-known/openid-configuration\n        status: 404\n        note: >-\n          Probed for an OIDC discovery document; the\
  \ CAS server returns a JSON 404\n          ({\"error\":\"Not Found\"}). No OpenID Connect surface is published.\n  - name: ShibbolethSaml\n    type: saml\n    operator: institution\n    applies_to: https://idp.nju.edu.cn/idp/shibboleth\n    description: >-\n      SAML 2.0 web SSO through NJU's own Shibboleth IdP, registered in CARSI and republished to\n      eduGAIN. Used in production by the university library for off-campus access to licensed\n      resources. Metadata is public; assertions require an NJU account.\n    evidence:\n      url: https://idp.nju.edu.cn/idp/shibboleth\n      status: 200\n    additional_evidence:\n      - url: https://idp.nju.edu.cn/idp/profile/SAML2/Redirect/SSO\n        status: 400\n        note: correct protocol rejection of a request carrying no SAMLRequest\n  - name: BookStackApiToken\n    type: bearer\n    operator: institution\n    applies_to: https://doc.nju.edu.cn/api\n    description: >-\n      The e-Science Document service publishes complete REST\
  \ API documentation publicly at\n      /api/docs — 79 endpoints across books, chapters, pages, shelves, attachments, images, users,\n      roles, recycle-bin, audit-log and search, with GET/POST/PUT/DELETE. The API itself is\n      token-gated: an unauthenticated call returns a clean JSON error envelope,\n      {\"error\":{\"message\":\"No authorization token found on the request\",\"code\":401}}. Tokens are\n      issued to NJU account holders from the user profile; there is no public registration. The\n      machine-readable description at /api/docs.json is itself behind the token, so the only\n      public description of this API is the HTML page.\n    evidence:\n      url: https://doc.nju.edu.cn/api/books\n      status: 401\n    additional_evidence:\n      - url: https://doc.nju.edu.cn/api/docs\n        status: 200\n        note: public HTML API reference\n      - url: https://doc.nju.edu.cn/api/docs.json\n        status: 401\n        note: the JSON description of the API requires\
  \ the token the API requires\n  - name: AnubisBotChallenge\n    type: challenge\n    operator: institution\n    applies_to: https://git.nju.edu.cn/api/v4\n    description: >-\n      NJU's GitLab instance sits behind an Anubis proof-of-work bot challenge. Every /api/v4 route\n      answers HTTP 200 with the challenge page (\"Making sure you're not a bot!\") to a non-browser\n      client, so the API is live and gated rather than dead or absent — the university's own mirror\n      site calls https://git.nju.edu.cn/api/v4/projects/2412/issues from a browser to render its\n      announcements. This is an anti-crawler control, not an authorization scheme; it is recorded\n      here because it is what a client encounters first.\n    evidence:\n      url: https://git.nju.edu.cn/api/v4/projects/2412/issues\n      status: 200\n      note: 200 body is the Anubis challenge, not the resource\n  - name: CampusNetworkGate\n    type: challenge\n    operator: institution\n    applies_to: https://opac.nju.edu.cn\n\
  \    description: >-\n      The library OPAC is restricted to the campus network: every route, including\n      /oai?verb=Identify, returns HTTP 403 with the body \"请使用南大VPN访问!\" (\"please access via the\n      NJU VPN\"). Live and gated by network location, not credentials.\n    evidence:\n      url: https://opac.nju.edu.cn/\n      status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanjing/refs/heads/main/authentication/nanjing-authentication.yml
summary_line: none/saml/cas/bearer/challenge · 9 schemes
tags:
- University
- Higher Education
- Education
- China
- C9 League
- Research
- Identity Federation
- Authentication
- Single Sign-On
- Research Computing
- Open Source Mirror
- Version Control
- Library
---
