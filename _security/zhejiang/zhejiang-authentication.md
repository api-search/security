---
api_key_in: []
api_specs:
- filename: zhejiang-mirror-service-openapi.yml
  format: yaml
  label: Open Source Software Mirror Service (MirrorZ catalog)
  slug: mirrors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/openapi/zhejiang-mirror-service-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Zhejiang Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zhejiang University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Zhejiang University
provider_slug: zhejiang
scheme_count: 0
schemes: []
slug: zhejiang-authentication
source_filename: zhejiang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# Zhejiang University — authentication posture across institution-operated surfaces\ngenerated: '2026-08-19'\nmethod: probed\nsource: Live probes 2026-08-19 of zju.edu.cn hosts; no vendor documentation was used.\nx-operator: institution\nsummary: >-\n  ZJU runs two institution-operated authentication surfaces — a CAS single sign-on\n  platform and a Shibboleth SAML 2.0 Identity Provider — and one institution-operated\n  public service that requires no authentication at all (the open source mirror).\n  There is no OAuth 2.0 authorization server, no API key issuance, and no developer\n  self-service credential flow anywhere on the public zju.edu.cn surface.\nsurfaces:\n  - name: Unified Identity Authentication (CAS)\n    x-operator: institution\n    host: zjuam.zju.edu.cn\n    type: CAS\n    protocol: Central Authentication Service (web SSO)\n    public_registration: false\n    machine_readable_metadata: false\n    evidence:\n      - url: https://zjuam.zju.edu.cn/cas/login?locale=en\n\
  \        status: 200\n        detail: >-\n          CAS login page, title \"Unified identity authentication platform\", bilingual\n          (zh-CN default, ?locale=en). Interactive login only — username/password,\n          QR-code scan and third-party IdP hand-off. No published API contract, no\n          service-registration endpoint reachable unauthenticated.\n  - name: Shibboleth Identity Provider\n    x-operator: institution\n    host: idp.zju.edu.cn\n    type: SAML2 IdP\n    entity_id: https://idp.zju.edu.cn/idp/shibboleth\n    machine_readable_metadata: true\n    metadata_url: https://idp.zju.edu.cn/idp/shibboleth\n    evidence:\n      - url: https://idp.zju.edu.cn/idp/shibboleth\n        status: 200\n        content_type: application/xml;charset=UTF-8\n        detail: SAML 2.0 EntityDescriptor, 14402 bytes, KeyDescriptor present.\n    endpoints:\n      single_sign_on:\n        - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n          location: https://idp.zju.edu.cn/idp/profile/Shibboleth/SSO\n\
  \        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://idp.zju.edu.cn/idp/profile/SAML2/POST/SSO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n          location: https://idp.zju.edu.cn/idp/profile/SAML2/POST-SimpleSign/SSO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://idp.zju.edu.cn/idp/profile/SAML2/Redirect/SSO\n      single_logout:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://idp.zju.edu.cn/idp/profile/SAML2/Redirect/SLO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://idp.zju.edu.cn/idp/profile/SAML2/POST/SLO\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n          location: https://idp.zju.edu.cn:8443/idp/profile/SAML2/SOAP/SLO\n      artifact_resolution:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n          location: https://idp.zju.edu.cn:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n\
  \        - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding\n          location: https://idp.zju.edu.cn:8443/idp/profile/SAML1/SOAP/ArtifactResolution\n      attribute_query:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n          location: https://idp.zju.edu.cn:8443/idp/profile/SAML2/SOAP/AttributeQuery\n        - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding\n          location: https://idp.zju.edu.cn:8443/idp/profile/SAML1/SOAP/AttributeQuery\n    caveat: >-\n      The served metadata carries the stock Shibboleth \"This is example metadata only\"\n      banner, which the distribution ships and many production IdPs never strip. The\n      endpoints it advertises resolve to the live IdP, so the document is treated as\n      the operating entity descriptor while the banner is recorded as-is rather than\n      edited away.\n  - name: Open Source Software Mirror\n    x-operator: institution\n    host: mirrors.zju.edu.cn\n    type: none\n    public_registration:\
  \ not_applicable\n    evidence:\n      - url: https://mirrors.zju.edu.cn/mirrorz.json\n        status: 200\n        detail: >-\n          Anonymous read. No Authorization header required, no WWW-Authenticate on the\n          response, no API key parameter. Response headers observed: server, date,\n          content-type, content-length, last-modified, etag, x-storage, accept-ranges.\n          No CORS header (Access-Control-Allow-Origin absent) — browser-side\n          cross-origin consumption is therefore blocked.\nnot_found:\n  - oauth2_authorization_server\n  - openid_connect_discovery\n  - api_key_issuance\n  - developer_self_service_portal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/authentication/zhejiang-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- China
- C9 League
- Double First-Class
- Identity Federation
- Single Sign-On
- Open Source Mirror
- Library
---
