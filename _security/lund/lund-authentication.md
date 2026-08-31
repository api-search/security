---
api_key_in: []
api_specs:
- filename: lund-publication-api-openapi.yml
  format: yaml
  label: Lund University Publications Search API
  slug: lund-publication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lund/refs/heads/main/openapi/lund-publication-api-openapi.yml
- filename: lund-student-papers-api-openapi.yml
  format: yaml
  label: LUP Student Papers Search API
  slug: lup-student-papers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lund/refs/heads/main/openapi/lund-student-papers-api-openapi.yml
auth_types:
- none
- saml
description: ''
kind: authentication
layout: security
method: probed
name: Lund Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lund University secures its APIs with none and saml across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lund University
provider_slug: lund
scheme_count: 2
schemes:
- description: 'No authentication. Confirmed by anonymous HTTP GET returning 200 with real data on: the LUP Search API, both OAI-PMH repositories, both SRU services, both unAPI services, the RSS feeds, the bulk export endpoint and the published JSON Schema.'
  name: none
  sources:
  - https://lup.lub.lu.se/search/publication?q=dna&format=json
  - https://lup.lub.lu.se/oai?verb=Identify
  - https://lup.lub.lu.se/sru?operation=searchRetrieve&version=1.1&query=dna
  - https://lup.lub.lu.se/search/unapi
  - https://lup.lub.lu.se/student-papers/search/publication?q=dna&format=json
  - https://lup.lub.lu.se/student-papers/oai?verb=Identify
  type: none
- description: SAML 2.0 / Shibboleth single sign-on against Lund's own Identity Provider (entityID https://idpv4.lu.se/idp/shibboleth, scope lu.se), registered in the Swedish national federation SWAMID and interfederated through eduGAIN. This is the gate in front of staff and student services — it authenticates people with an institutional affiliation, and it is not an API credential a third-party developer can obtain.
  name: swamid-saml-sso
  sources:
  - https://idpv4.lu.se/idp/shibboleth
  - https://mds.swamid.se/md/swamid-idp.xml
  type: saml
slug: lund-authentication
source_filename: lund-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live anonymous probes of every Lund University surface on this profile, 2026-08-30.\nsummary:\n  types:\n  - none\n  - saml\nnote: >-\n  Lund University's public machine-readable surfaces are entirely anonymous — no key, no\n  token, no registration. Everything that is gated is gated by federated institutional\n  affiliation (SWAMID SAML), not by an API credential, which is the characteristic access\n  model of a university rather than a commercial API provider. There is no developer\n  registration flow, no self-service key issuance, and no plan to buy.\nschemes:\n- name: none\n  type: none\n  description: >-\n    No authentication. Confirmed by anonymous HTTP GET returning 200 with real data on:\n    the LUP Search API, both OAI-PMH repositories, both SRU services, both unAPI services,\n    the RSS feeds, the bulk export endpoint and the published JSON Schema.\n  sources:\n  - https://lup.lub.lu.se/search/publication?q=dna&format=json\n\
  \  - https://lup.lub.lu.se/oai?verb=Identify\n  - https://lup.lub.lu.se/sru?operation=searchRetrieve&version=1.1&query=dna\n  - https://lup.lub.lu.se/search/unapi\n  - https://lup.lub.lu.se/student-papers/search/publication?q=dna&format=json\n  - https://lup.lub.lu.se/student-papers/oai?verb=Identify\n- name: swamid-saml-sso\n  type: saml\n  description: >-\n    SAML 2.0 / Shibboleth single sign-on against Lund's own Identity Provider\n    (entityID https://idpv4.lu.se/idp/shibboleth, scope lu.se), registered in the Swedish\n    national federation SWAMID and interfederated through eduGAIN. This is the gate in\n    front of staff and student services — it authenticates people with an institutional\n    affiliation, and it is not an API credential a third-party developer can obtain.\n  sources:\n  - https://idpv4.lu.se/idp/shibboleth\n  - https://mds.swamid.se/md/swamid-idp.xml\ngated:\n- surface: LUCRIS / Research Portal Pure web service\n  url: https://portal.research.lu.se/ws/api\n \
  \ observed_status: 500\n  observed_body: '{\"timestamp\":...,\"status\":999,\"error\":\"None\"}'\n  detail: >-\n    The Elsevier Pure web service path exists on Lund's portal host but refuses anonymous\n    callers with an HTTP 500 carrying Pure's status 999 envelope. Lund documents that LUCRIS\n    content can be retrieved via API for institutional reporters and web editors; there is\n    no open self-service route to a key, and the contract is Elsevier's in any case.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lund/refs/heads/main/authentication/lund-authentication.yml
summary_line: none/saml · 2 schemes
tags:
- University
- Higher Education
- Education
- Sweden
- Europe
- Research
- Research Repository
- Publications
- Library
- Open Metadata
- Identity Federation
- OAI-PMH
---
