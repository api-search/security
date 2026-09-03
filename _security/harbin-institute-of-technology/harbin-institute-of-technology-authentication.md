---
api_key_in: []
auth_types: []
description: Authentication posture across the surfaces Harbin Institute of Technology actually exposes. Re-authored 2026-09-01 from live probes. The previous version of this file was DERIVED from Elsevier's Pure OpenAPI document and described Elsevier's api-key scheme as though it were HIT's; it was removed along with the rest of the vendor-derived set.
kind: authentication
layout: security
method: probed
name: Harbin Institute Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbin Institute of Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Harbin Institute of Technology
provider_slug: harbin-institute-of-technology
scheme_count: 0
schemes: []
slug: harbin-institute-of-technology-authentication
source_filename: harbin-institute-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# authorship: hand-authored by API Evangelist tooling from live HTTP probes,\n# 2026-09-01 university pipeline run. `method: probed` below is the university\n# contract's vocabulary; x-method carries the value the provenance manifest reads.\nx-method: manual\ngenerated: '2026-09-01'\nmethod: probed\nsource: live HTTP probes of scholar.hit.edu.cn and idp.hit.edu.cn, 2026-09-01\ndescription: >-\n  Authentication posture across the surfaces Harbin Institute of Technology actually exposes.\n  Re-authored 2026-09-01 from live probes. The previous version of this file was DERIVED from\n  Elsevier's Pure OpenAPI document and described Elsevier's api-key scheme as though it were HIT's;\n  it was removed along with the rest of the vendor-derived set.\nsurfaces:\n- name: HIT research portal OAI-PMH endpoint\n  url: https://scholar.hit.edu.cn/ws/oai\n  x-operator: tenant\n  auth: none\n  anonymous: true\n  evidence:\n  - url: https://scholar.hit.edu.cn/ws/oai?verb=ListRecords&metadataPrefix=oai_dc&set=publications:all\n\
  \    status: 200\n    detail: 358,884 bytes of records returned with no credential presented.\n- name: HIT research portal RSS feeds\n  url: https://scholar.hit.edu.cn/en/publications/?format=rss\n  x-operator: tenant\n  auth: none\n  anonymous: true\n  evidence:\n  - url: https://scholar.hit.edu.cn/en/publications/?format=rss\n    status: 200\n    detail: application/rss+xml, 108,758 bytes, RSS 2.0 with Dublin Core extensions.\n  - url: https://scholar.hit.edu.cn/en/persons/?format=rss\n    status: 200\n    detail: application/rss+xml, 51,699 bytes.\n- name: Elsevier Pure web services API (vendor contract, HIT tenancy)\n  url: https://scholar.hit.edu.cn/ws/api\n  x-operator: tenant\n  auth: api_key\n  anonymous: false\n  detail: >-\n    The Pure API is deployed on HIT's host but is NOT anonymously callable. The unversioned\n    OpenAPI document is served without a credential; every data path returns 401. The api-key\n    scheme is Elsevier's, issued per Pure customer, and is not an HIT-operated\
  \ credential.\n    No HIT-facing request process for a key was found.\n  evidence:\n  - url: https://scholar.hit.edu.cn/ws/api/research-outputs?size=1\n    status: 401\n    detail: 'application/problem+json — {\"title\":\"Request not authorized.\",\"detail\":\"Full authentication is required to access this resource\"}'\n  - url: https://scholar.hit.edu.cn/ws/api/524.0/openapi.json\n    status: 401\n    detail: Versioned contract itself is credential-gated.\n  - url: https://scholar.hit.edu.cn/ws/api/openapi.json\n    status: 200\n    detail: >-\n      Unversioned contract IS served anonymously — and it is Elsevier's, titled \"Pure API\",\n      contact pure-support@elsevier.com, 827 paths. Not HIT's contract.\n- name: HIT Shibboleth Identity Provider\n  url: https://idp.hit.edu.cn/idp/shibboleth\n  x-operator: institution\n  auth: saml2\n  anonymous: false\n  detail: >-\n    HIT's own SAML 2.0 IdP. Metadata document is served anonymously; authentication itself is\n    institutional credential\
  \ against HIT's directory. This is the one authentication surface in\n    this repo that HIT operates rather than rents.\n  entity_id: https://idp.hit.edu.cn/idp/shibboleth\n  scope: hit.edu.cn\n  bindings:\n  - HTTP-Redirect\n  - HTTP-POST\n  - HTTP-POST-SimpleSign\n  - SOAP\n  evidence:\n  - url: https://idp.hit.edu.cn/idp/shibboleth\n    status: 200\n    detail: SAML 2.0 EntityDescriptor, 14,377 bytes, IDPSSODescriptor + AttributeAuthorityDescriptor.\n  - url: https://idp.hit.edu.cn/idp/profile/SAML2/Redirect/SSO\n    status: 400\n    detail: Live SSO handler rejecting a bare GET with no SAMLRequest.\n- name: HIT unified identity authentication platform (统一身份认证平台)\n  url: https://ids.hit.edu.cn/\n  x-operator: institution\n  auth: institutional_login\n  anonymous: false\n  detail: >-\n    Campus SSO front door for staff and students. Interactive login only; no documented\n    machine interface and no published API. Recorded as a surface, not as an API.\n  evidence:\n  - url: https://ids.hit.edu.cn/\n\
  \    status: 200\n    detail: HTML login page, title 统一身份认证平台.\nnotes:\n- >-\n  No HIT-issued API credential of any kind was found. Every credential-gated surface here is\n  gated by either Elsevier (Pure api-key) or campus identity (SAML / SSO). There is no\n  developer key-issuance process to document because there is no HIT developer programme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbin-institute-of-technology/refs/heads/main/authentication/harbin-institute-of-technology-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- China
- Technical University
- C9 League
- Research
- Scholarly
- Identity Federation
- Research Repository
- OAI-PMH
---
