---
api_key_in: []
api_specs:
- filename: postech-oasis-oai-pmh-openapi.yml
  format: yaml
  label: POSTECH OASIS Repository OAI-PMH
  slug: oasis-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postech/refs/heads/main/openapi/postech-oasis-oai-pmh-openapi.yml
auth_types: []
description: 'How POSTECH''s institution-operated machine-readable surfaces authenticate. Three distinct regimes are in play and they do not resemble a company''s: the OASIS repository''s OAI-PMH harvesting endpoint is fully anonymous, the PLMS Moodle Web Services REST interface is token-gated and returns a Moodle fault to anyone without one, and the LTI 1.3 platform on the same LMS runs a standards-defined OAuth 2.0 client-credentials flow with a signed JWT assertion. Separately, POSTECH operates its own SAML 2.0 identity provider for browser sign-in to campus services — federation infrastructure, not an API credential. Nothing on this surface is self-service for an outside developer.'
kind: authentication
layout: security
method: probed
name: Postech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pohang University of Science and Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Pohang University of Science and Technology
provider_slug: postech
scheme_count: 0
schemes: []
slug: postech-authentication
source_filename: postech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Pohang University of Science and Technology — Authentication\ndescription: >-\n  How POSTECH's institution-operated machine-readable surfaces authenticate. Three distinct regimes\n  are in play and they do not resemble a company's: the OASIS repository's OAI-PMH harvesting\n  endpoint is fully anonymous, the PLMS Moodle Web Services REST interface is token-gated and\n  returns a Moodle fault to anyone without one, and the LTI 1.3 platform on the same LMS runs a\n  standards-defined OAuth 2.0 client-credentials flow with a signed JWT assertion. Separately,\n  POSTECH operates its own SAML 2.0 identity provider for browser sign-in to campus services —\n  federation infrastructure, not an API credential. Nothing on this surface is self-service for an\n  outside developer.\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of oasis.postech.ac.kr, plms.postech.ac.kr and idpass.postech.ac.kr\n  on 2026-08-30. No POSTECH-published authentication\
  \ documentation was found.\nx-operator: institution\nurl: https://raw.githubusercontent.com/api-evangelist/postech/main/authentication/postech-authentication.yml\n\nmechanisms:\n  - id: oai-pmh-anonymous\n    type: none\n    label: OASIS OAI-PMH — no authentication\n    applies_to:\n      - POSTECH OASIS Repository OAI-PMH\n    detail: >-\n      https://oasis.postech.ac.kr/oai/request accepts and requires no credential. Identify,\n      ListMetadataFormats, ListSets and ListRecords all returned 200 with full payloads to an\n      anonymous client. This path is also exempt from the JavaScript bot challenge that fronts the\n      rest of the host, which is the single most useful fact about POSTECH's programmable surface.\n    method: probed\n    source: https://oasis.postech.ac.kr/oai/request?verb=Identify\n\n  - id: moodle-webservice-token\n    type: apiKey\n    label: PLMS Moodle Web Services — wstoken\n    in: query\n    parameter_names:\n      - wstoken\n    applies_to:\n      - POSTECH\
  \ LMS (PLMS) Moodle Web Services\n    detail: >-\n      https://plms.postech.ac.kr/webservice/rest/server.php is live and answers an anonymous call\n      with a moodle_exception errorcode invalidtoken (\"잘못된 토큰 - 토큰이 발견되지 않았습니다\"),\n      confirming the web services subsystem is enabled. Tokens are issued inside Moodle to\n      authenticated POSTECH accounts; there is no public registration, no documented scope catalog\n      and no external developer program.\n    onboarding: >-\n      Not available to the public. A token is created by a POSTECH-account holder through the LMS\n      itself or by an administrator; no self-service issuance surface was found.\n    method: probed\n    source: https://plms.postech.ac.kr/webservice/rest/server.php?wsfunction=core_webservice_get_site_info&moodlewsrestformat=json\n\n  - id: lti13-client-credentials\n    type: oauth2\n    label: PLMS LTI 1.3 platform — OAuth 2.0 client credentials with signed JWT\n    flow: clientCredentials\n    token_url:\
  \ https://plms.postech.ac.kr/mod/lti/token.php\n    jwks_url: https://plms.postech.ac.kr/mod/lti/certs.php\n    applies_to:\n      - POSTECH LMS (PLMS) LTI 1.3 Advantage platform\n    detail: >-\n      The standards-defined LTI Advantage service authentication: a registered tool presents a\n      client_assertion JWT signed with its own key and receives a bearer access token scoped to the\n      LTI Advantage services. POSTECH's platform keyset at /mod/lti/certs.php is public (RSA,\n      RS256, kid 13acf24233904ff6db00), which is exactly what a tool needs to verify POSTECH-issued\n      id_tokens. The token endpoint returns {\"error\":\"invalid_request\"} to an unparameterised\n      request. Tool registration is not open — it is an LMS administrator action.\n    method: probed\n    source: https://plms.postech.ac.kr/mod/lti/token.php\n\n  - id: saml2-sso\n    type: saml\n    label: POSTECH identity provider — SAML 2.0 web browser SSO\n    sso_url: https://idpass.postech.ac.kr/simplesaml/saml2/idp/SSOService.php\n\
  \    slo_url: https://idpass.postech.ac.kr/simplesaml/saml2/idp/SingleLogoutService.php\n    entity_id: https://idpass.postech.ac.kr/idp/simplesamlphp\n    applies_to:\n      - POSTECH SAML 2.0 Identity Provider\n    detail: >-\n      Browser-profile SSO for POSTECH accounts, scoped to postech.ac.kr, registered in the KAFE\n      federation and reachable through eduGAIN. Supports the REFEDS Research and Scholarship entity\n      category and asserts SIRTFI, with a REFEDS security contact in metadata. This authenticates\n      people to services, not clients to APIs, and is recorded here because it is machine-readable\n      institutional infrastructure — not because it issues API credentials.\n    method: probed\n    source: https://technical.edugain.org/api.php?action=show_entity&entityid=https://idpass.postech.ac.kr/idp/simplesamlphp&format=json\n\nblocked:\n  - id: dspace-rest\n    label: OASIS DSpace REST (/rest, /server/api)\n    detail: >-\n      Both DSpace REST roots return HTTP\
  \ 200 carrying a JavaScript challenge shell\n      (data-name=\"js-challenge\", noscript text in Korean) rather than a HAL/JSON payload. This is a\n      bot-management layer in front of the repository, not an authentication scheme and not a dead\n      host — an ordinary browser would pass it. No REST contract could be observed, so none is\n      recorded.\n    evidence:\n      - url: https://oasis.postech.ac.kr/server/api\n        status: 200\n      - url: https://oasis.postech.ac.kr/rest/communities\n        status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postech/refs/heads/main/authentication/postech-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- South Korea
- Korea
- Asia
- Private Research University
- Research
- Research Data
- Institutional Repository
- OAI-PMH
- DSpace
- Library
- Identity Federation
- SAML
- eduGAIN
- LTI
- Learning Management System
- Course Catalog
---
