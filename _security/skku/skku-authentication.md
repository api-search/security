---
api_key_in: []
auth_types:
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Skku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sungkyunkwan University secures its APIs with saml2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sungkyunkwan University
provider_slug: skku
scheme_count: 1
schemes:
- assurance:
  - https://refeds.org/sirtfi
  bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  description: SKKU's institutional SAML 2.0 identity provider, running SimpleSAMLphp on SKKU's own kafe.skku.edu host. It supports the REFEDS Research and Scholarship entity category and asserts the REFEDS Sirtfi security incident response assurance profile. Signing and encryption use a self-issued X.509 certificate (CN=kafe.skku.edu, O=SKKU, OU=Information Service Affairs Team, valid 2022-09-23 to 2032-09-22).
  endpoints:
    single_logout: https://kafe.skku.edu/simplesaml/saml2/idp/SingleLogoutService.php
    single_sign_on: https://kafe.skku.edu/simplesaml/saml2/idp/SSOService.php
  entity_categories_supported:
  - http://refeds.org/category/research-and-scholarship
  entity_id: https://kafe.skku.edu/idp/simplesamlphp
  liveness:
  - note: Probed 2026-09-01. SimpleSAMLphp answers "No SAML request provided — You accessed the Single Sign On Service interface, but did not provide a SAML Authentication Request", with a session tracking number. A 400 here is the correct response to a request carrying no SAMLRequest, so the advertised endpoint is confirmed live and functioning rather than dead.
    status: 400
    url: https://kafe.skku.edu/simplesaml/saml2/idp/SSOService.php
  name: kafeSamlIdP
  name_id_formats:
  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient
  protocol: urn:oasis:names:tc:SAML:2.0:protocol
  registration:
    authority: http://kafe.kreonet.net
    federation: KAFE (Korea Access Federation), interfederated through eduGAIN
    first_seen_in_edugain: '2022-11-16'
    jurisdiction: KR
    policy: https://www.kafe.or.kr/kafe-mrps-v1.1.pdf
    registered: '2022-09-26'
  scope: skku.edu
  sources:
  - examples/skku-idp-saml-entity-descriptor-example.xml
  type: saml2
  x-note: The IdP's own metadata paths are not directly retrievable — https://kafe.skku.edu/ returns 200 but /idp/simplesamlphp and /simplesaml/saml2/idp/metadata.php return a Korean WAF interstitial ("정보보호를 위해 부적절한 접근이 차단 되었습니다", HTTP 404). The metadata is published through the federation aggregate instead, which is the normal and correct distribution channel for it.
  x-operator: institution
slug: skku-authentication
source_filename: skku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  examples/skku-idp-saml-entity-descriptor-example.xml, retrieved 2026-09-01 from the eduGAIN\n  metadata database; plus live probes of pure.skku.edu, icampus.skku.edu, sugang.skku.edu and\n  kingo.skku.edu.\nnote: >-\n  Sungkyunkwan University publishes no developer-facing authorization surface. There is no client\n  registration path, no token endpoint, no consent screen and no API key issuance an outside\n  developer could integrate against. What it does operate is an END-USER identity federation, and\n  that is a different thing — it is recorded here because it is the strongest machine-readable\n  surface the institution runs, not because it is consumable by a third-party integrator.\nsummary:\n  types:\n  - saml2\n  developer_usable: false\n  public_client_registration: false\n  token_endpoint: false\nschemes:\n- name: kafeSamlIdP\n  type: saml2\n  x-operator: institution\n  entity_id: https://kafe.skku.edu/idp/simplesamlphp\n\
  \  scope: skku.edu\n  protocol: urn:oasis:names:tc:SAML:2.0:protocol\n  name_id_formats:\n  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  endpoints:\n    single_sign_on: https://kafe.skku.edu/simplesaml/saml2/idp/SSOService.php\n    single_logout: https://kafe.skku.edu/simplesaml/saml2/idp/SingleLogoutService.php\n  registration:\n    authority: http://kafe.kreonet.net\n    federation: KAFE (Korea Access Federation), interfederated through eduGAIN\n    registered: '2022-09-26'\n    first_seen_in_edugain: '2022-11-16'\n    policy: https://www.kafe.or.kr/kafe-mrps-v1.1.pdf\n    jurisdiction: KR\n  assurance:\n  - https://refeds.org/sirtfi\n  entity_categories_supported:\n  - http://refeds.org/category/research-and-scholarship\n  description: >-\n    SKKU's institutional SAML 2.0 identity provider, running SimpleSAMLphp on SKKU's own\n    kafe.skku.edu host.\
  \ It supports the REFEDS Research and Scholarship entity category and asserts\n    the REFEDS Sirtfi security incident response assurance profile. Signing and encryption use a\n    self-issued X.509 certificate (CN=kafe.skku.edu, O=SKKU, OU=Information Service Affairs Team,\n    valid 2022-09-23 to 2032-09-22).\n  liveness:\n  - url: https://kafe.skku.edu/simplesaml/saml2/idp/SSOService.php\n    status: 400\n    note: >-\n      Probed 2026-09-01. SimpleSAMLphp answers \"No SAML request provided — You accessed the Single\n      Sign On Service interface, but did not provide a SAML Authentication Request\", with a session\n      tracking number. A 400 here is the correct response to a request carrying no SAMLRequest, so\n      the advertised endpoint is confirmed live and functioning rather than dead.\n  sources:\n  - examples/skku-idp-saml-entity-descriptor-example.xml\n  x-note: >-\n    The IdP's own metadata paths are not directly retrievable — https://kafe.skku.edu/ returns 200\n   \
  \ but /idp/simplesamlphp and /simplesaml/saml2/idp/metadata.php return a Korean WAF interstitial\n    (\"정보보호를 위해 부적절한 접근이 차단 되었습니다\", HTTP 404). The metadata is published through the\n    federation aggregate instead, which is the normal and correct distribution channel for it.\ngated_surfaces:\n- name: Kingo Portal (single sign-on)\n  url: https://www.skku.edu/eng/CampusLife/ITServices/KingoPortal1_1.do\n  x-operator: institution\n  note: >-\n    The campus SSO environment fronting Gmail/Google Workspace, GLS, iCampus, electronic approval and\n    notice boards. Enrolment-gated; no public authentication API, no developer registration, no\n    published rate limits.\n- name: Pure Web Service\n  url: https://pure.skku.edu/ws/api\n  x-operator: tenant\n  note: >-\n    https://pure.skku.edu/ws/api/524/ returns HTTP 401 \"Request not authorized. Please provide a\n    valid API key for access.\" The documentation page at /ws/api canonicalises to\n    https://api.elsevierpure.com/ws/api/documentation/index.html\
  \ — this is Elsevier's contract on\n    SKKU's tenancy, and no key issuance path for third parties was found.\n- name: iCampus\n  url: https://icampus.skku.edu/\n  x-operator: institution\n  note: >-\n    Learning system on SKKU's own domain, a Laravel application. /api/v1/courses returns 419\n    \"Page Expired\" (CSRF), every other API path returns the app's Korean 404. No public API.\n- name: Course registration (수강신청)\n  url: https://sugang.skku.edu/\n  x-operator: institution\n  note: HTTP 200, Korean-only, session-gated. No machine-readable course catalog is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skku/refs/heads/main/authentication/skku-authentication.yml
summary_line: saml2 · 1 scheme
tags:
- University
- Higher Education
- Education
- Research
- South Korea
- Seoul
- Identity Federation
- SAML
- eduGAIN
- Research Repository
- OAI-PMH
- Open Access
---
