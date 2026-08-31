---
api_key_in: []
api_specs:
- filename: snu-oai-pmh-api-openapi.yml
  format: yaml
  label: Seoul National University OAI PMH API
  slug: snu-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/openapi/snu-oai-pmh-api-openapi.yml
- filename: snu-opensearch-api-openapi.yml
  format: yaml
  label: Seoul National University Open Search API
  slug: snu-opensearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/openapi/snu-opensearch-api-openapi.yml
auth_types:
- none
- saml2
description: Seoul National University issues no API keys, runs no developer registration, and publishes no OAuth or OIDC authorization server for any public surface. Its two machine-readable interfaces are anonymous by design, and its one credentialed surface is a federation Identity Provider that authenticates SNU's own people to other organizations' services — not an API SNU sells access to.
kind: authentication
layout: security
method: probed
name: Snu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seoul National University secures its APIs with none and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Seoul National University
provider_slug: snu
scheme_count: 3
schemes:
- applies_to:
  - https://s-space.snu.ac.kr/oai/request
  - https://s-space.snu.ac.kr/oai/driver
  - https://s-space.snu.ac.kr/oai/openaire
  - https://kossda.snu.ac.kr/oai/request
  - https://kossda.snu.ac.kr/oai/driver
  description: Both OAI-PMH data providers are open and unauthenticated. Verified anonymously with no cookie, no header and no credential of any kind.
  name: none
  sources:
  - openapi/snu-s-space-oai-pmh-openapi.yml
  - openapi/snu-kossda-oai-pmh-openapi.yml
  type: none
- applies_to:
  - https://s-space.snu.ac.kr/open-search/
  - https://s-space.snu.ac.kr/open-search/description.xml
  - https://s-space.snu.ac.kr/feed/atom_1.0/site
  - https://s-space.snu.ac.kr/feed/rss_2.0/site
  cookie_name: js-challenge
  description: NOT authentication and must not be scored as such — a bot-mitigation interstitial. s-space.snu.ac.kr and kossda.snu.ac.kr front their web and OpenSearch paths with a JavaScript challenge that returns HTTP 200 and a ~1 KB HTML shell carrying a `data-token`; the client must set that token as the `js-challenge` cookie (TTL 1800s) to receive real content. Recorded here because a machine client is blocked without it. The OAI-PMH paths are exempted from the challenge, which is the correct call.
  in: cookie
  name: jsChallengeCookie
  sources:
  - openapi/snu-s-space-opensearch-openapi.yml
  type: apiKey
- assurance_certifications:
  - https://refeds.org/sirtfi
  contacts:
    security: ym0427@snu.ac.kr
    technical: ercc_infra@snu.ac.kr
  description: 'SNU''s SAML 2.0 IdP, registered in the KAFE national federation (registrationAuthority http://kafe.kreonet.net, registrationInstant 2024-06-25) and exported into eduGAIN. SNU is the asserting party: this endpoint authenticates SNU staff and students to relying parties elsewhere. It is not an API SNU exposes for third-party consumption, and it accepts only federation-registered Service Providers, so it is unusable as a general developer surface.'
  endpoints:
    single_logout:
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
      location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleLogout
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
      location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleLogout
    single_sign_on:
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
      location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleSignOnService
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
      location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleSignOnService
  entity_categories:
  - http://refeds.org/category/research-and-scholarship
  entity_id: https://kafegw.snu.ac.kr/idp/simplesamlphp
  keys:
  - not_after: '2028-06-03'
    subject: CN=kafegw.snu.ac.kr, O=SNU, OU=Information Systems and Technology, L=Seoul, C=KR
    use: signing
  - not_after: '2028-06-03'
    subject: CN=kafegw.snu.ac.kr, O=SNU, OU=Information Systems and Technology, L=Seoul, C=KR
    use: encryption
  name: samlIdentityProvider
  name_id_formats:
  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient
  role: identity-provider
  scope: snu.ac.kr
  software: SimpleSAMLphp
  sources:
  - authentication/snu-kafe-saml-idp-metadata.xml
  type: saml2
slug: snu-authentication
source_filename: snu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  openapi/snu-s-space-oai-pmh-openapi.yml, openapi/snu-kossda-oai-pmh-openapi.yml,\n  openapi/snu-s-space-opensearch-openapi.yml, and\n  authentication/snu-kafe-saml-idp-metadata.xml (extracted from the eduGAIN aggregate).\n  All statements below were established by live probe on 2026-08-19.\nsummary:\n  types:\n    - none\n    - saml2\n  public_surfaces_require_no_credential: true\ndescription: >-\n  Seoul National University issues no API keys, runs no developer registration, and\n  publishes no OAuth or OIDC authorization server for any public surface. Its two\n  machine-readable interfaces are anonymous by design, and its one credentialed surface\n  is a federation Identity Provider that authenticates SNU's own people to other\n  organizations' services — not an API SNU sells access to.\nschemes:\n  - name: none\n    type: none\n    description: >-\n      Both OAI-PMH data providers are open and unauthenticated. Verified\
  \ anonymously\n      with no cookie, no header and no credential of any kind.\n    applies_to:\n      - https://s-space.snu.ac.kr/oai/request\n      - https://s-space.snu.ac.kr/oai/driver\n      - https://s-space.snu.ac.kr/oai/openaire\n      - https://kossda.snu.ac.kr/oai/request\n      - https://kossda.snu.ac.kr/oai/driver\n    sources:\n      - openapi/snu-s-space-oai-pmh-openapi.yml\n      - openapi/snu-kossda-oai-pmh-openapi.yml\n  - name: jsChallengeCookie\n    type: apiKey\n    in: cookie\n    cookie_name: js-challenge\n    description: >-\n      NOT authentication and must not be scored as such — a bot-mitigation interstitial.\n      s-space.snu.ac.kr and kossda.snu.ac.kr front their web and OpenSearch paths with a\n      JavaScript challenge that returns HTTP 200 and a ~1 KB HTML shell carrying a\n      `data-token`; the client must set that token as the `js-challenge` cookie (TTL 1800s)\n      to receive real content. Recorded here because a machine client is blocked without\n\
  \      it. The OAI-PMH paths are exempted from the challenge, which is the correct call.\n    applies_to:\n      - https://s-space.snu.ac.kr/open-search/\n      - https://s-space.snu.ac.kr/open-search/description.xml\n      - https://s-space.snu.ac.kr/feed/atom_1.0/site\n      - https://s-space.snu.ac.kr/feed/rss_2.0/site\n    sources:\n      - openapi/snu-s-space-opensearch-openapi.yml\n  - name: samlIdentityProvider\n    type: saml2\n    role: identity-provider\n    entity_id: https://kafegw.snu.ac.kr/idp/simplesamlphp\n    description: >-\n      SNU's SAML 2.0 IdP, registered in the KAFE national federation\n      (registrationAuthority http://kafe.kreonet.net, registrationInstant 2024-06-25) and\n      exported into eduGAIN. SNU is the asserting party: this endpoint authenticates SNU\n      staff and students to relying parties elsewhere. It is not an API SNU exposes for\n      third-party consumption, and it accepts only federation-registered Service\n      Providers, so it is unusable\
  \ as a general developer surface.\n    software: SimpleSAMLphp\n    endpoints:\n      single_sign_on:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleSignOnService\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleSignOnService\n      single_logout:\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n          location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleLogout\n        - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n          location: https://kafegw.snu.ac.kr/saml/module.php/saml/idp/singleLogout\n    name_id_formats:\n      - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n    scope: snu.ac.kr\n    entity_categories:\n      - http://refeds.org/category/research-and-scholarship\n    assurance_certifications:\n      - https://refeds.org/sirtfi\n\
  \    keys:\n      - use: signing\n        subject: CN=kafegw.snu.ac.kr, O=SNU, OU=Information Systems and Technology, L=Seoul, C=KR\n        not_after: '2028-06-03'\n      - use: encryption\n        subject: CN=kafegw.snu.ac.kr, O=SNU, OU=Information Systems and Technology, L=Seoul, C=KR\n        not_after: '2028-06-03'\n    contacts:\n      technical: ercc_infra@snu.ac.kr\n      security: ym0427@snu.ac.kr\n    sources:\n      - authentication/snu-kafe-saml-idp-metadata.xml\nfindings:\n  - id: idp-metadata-endpoint-500\n    severity: medium\n    detail: >-\n      The IdP does not serve its own metadata. The conventional SimpleSAMLphp path\n      https://kafegw.snu.ac.kr/saml/module.php/saml/idp/metadata.php returns HTTP 500, and\n      the entityID URL https://kafegw.snu.ac.kr/idp/simplesamlphp returns 404. The only\n      retrievable copy of SNU's SAML metadata is the KAFE/eduGAIN aggregate. A relying\n      party cannot self-serve it from SNU.\n  - id: idp-privacy-statement-dead\n  \
  \  severity: low\n    detail: >-\n      The mdui:PrivacyStatementURL published in SNU's own IdP metadata,\n      http://en.snu.ac.kr/upload/footer/privacy.pdf, returns HTTP 404. A federation\n      partner following SNU's declared privacy statement gets nothing. The live policy is\n      at https://en.snu.ac.kr/privacy-policy.\n  - id: registration-policy-soft-404\n    severity: low\n    detail: >-\n      The KAFE registration policy URL in the metadata,\n      https://www.kafe.or.kr/kafe-mrps-v1.1.pdf, returns HTTP 200 with 10,732 bytes of\n      HTML — the KAFE homepage, not a PDF. Soft-404. This is KAFE's defect, not SNU's,\n      but it is in the chain a relying party would follow.\n  - id: no-oauth-no-oidc\n    severity: informational\n    detail: >-\n      No /.well-known/openid-configuration, no /.well-known/oauth-authorization-server,\n      and no /.well-known/security.txt on www.snu.ac.kr (404 on each). No OAuth 2.0 or\n      OIDC surface exists for third-party developers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/authentication/snu-authentication.yml
summary_line: none/saml2 · 3 schemes
tags:
- University
- Higher Education
- Education
- South Korea
- Research
- Research Data
- Institutional Repository
- Research Repository
- Identity Federation
- OAI-PMH
- SAML
- Open Access
- Library
- National University
---
