---
api_key_in: []
api_specs:
- filename: fudan-identity-openapi.yml
  format: yaml
  label: Fudan University Unified Identity — OpenID Connect
  slug: identity-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/openapi/fudan-identity-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Fudan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fudan University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Fudan University
provider_slug: fudan
scheme_count: 0
schemes: []
slug: fudan-authentication
source_filename: fudan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "x-method: derived\nname: Fudan University — authentication surfaces\ngenerated: '2026-08-30'\nmethod: probed\nsource: live probes of id.fudan.edu.cn, idpfudan.fudan.edu.cn and rdr.fudan.edu.cn on 2026-08-30\nx-operator: institution\nsummary: >-\n  Fudan University operates its own identity infrastructure — an OpenID Connect provider\n  and a SAML 2.0 Shibboleth identity provider — on hosts under fudan.edu.cn. Both publish\n  machine-readable metadata without authentication. No API key programme, no public client\n  registration and no developer portal was found for either.\nmechanisms:\n  - type: openid_connect\n    operator: institution\n    issuer: https://id.fudan.edu.cn/idp\n    discovery: https://id.fudan.edu.cn/idp/.well-known/openid-configuration\n    jwks: https://id.fudan.edu.cn/idp/oidc/getPublicKey\n    authorization_endpoint: https://id.fudan.edu.cn/idp/authCenter/authenticate\n    token_endpoint: https://id.fudan.edu.cn/idp/oidc/getOidcToken\n    userinfo_endpoint:\
  \ https://id.fudan.edu.cn/idp/oidc/getUserInfo\n    grant_types: [ implicit, authorization_code, refresh_token ]\n    id_token_signing_alg_values: [ RS256, ES256, HS256 ]\n    client_registration: none published\n    evidence:\n      - url: https://id.fudan.edu.cn/idp/.well-known/openid-configuration\n        status: 200\n        content_type: application/json;charset=UTF-8\n      - url: https://id.fudan.edu.cn/idp/oidc/getPublicKey\n        status: 200\n        content_type: application/json;charset=UTF-8\n        note: One RSA key returned, kid RS256.\n  - type: saml2\n    operator: institution\n    entity_id: https://idpfudan.fudan.edu.cn/idp/shibboleth\n    metadata: https://idpfudan.fudan.edu.cn/idp/shibboleth\n    software: Shibboleth Identity Provider\n    scope: fudan.edu.cn\n    federation: CARSI (https://www.carsi.edu.cn), interfederated into eduGAIN\n    roles: [ IDPSSODescriptor, AttributeAuthorityDescriptor ]\n    protocols:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n\
  \      - urn:oasis:names:tc:SAML:1.1:protocol\n      - urn:mace:shibboleth:1.0\n    evidence:\n      - url: https://idpfudan.fudan.edu.cn/idp/shibboleth\n        status: 200\n        content_type: application/xml;charset=UTF-8\n        note: 14,734-byte SAML 2.0 EntityDescriptor, captured to examples/fudan-idp-saml-metadata.xml.\n      - url: https://technical.edugain.org/api.php?action=list_entities&format=json\n        status: 200\n        note: >-\n          eduGAIN entity id 671764, registration authority https://www.carsi.edu.cn,\n          display name \"Fudan University\" / \"复旦大学\", scope fudan.edu.cn, first seen\n          2020-02-12.\n  - type: session_cookie\n    operator: institution\n    surface: https://rdr.fudan.edu.cn/datahome/\n    note: >-\n      The research data platform's JSON backend is session based and additionally requires\n      an application-specific state parameter. Unauthenticated calls return HTTP 200 with\n      a JSON refusal rather than a 401. See errors/fudan-errors.yml.\n\
  \    evidence:\n      - url: https://rdr.fudan.edu.cn/datahome/open/admin/loginUserInfo.do\n        status: 200\n        note: 'Body: {\"status\":4000,\"message\":\"状态锁不得为空\",\"data\":null}'\nnot_found:\n  - Public API key issuance or developer account registration.\n  - Any published OAuth client registration path.\n  - A SAML metadata document served by id.fudan.edu.cn itself (404 on /idp/shibboleth, /idp/saml2/metadata, /idp/profile/SAML2/Metadata, /idp/metadata.xml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/authentication/fudan-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- China
- Shanghai
- C9 League
- Identity Federation
- Research Data
- Single Sign-On
---
