---
api_key_in: []
api_specs:
- filename: kyushu-qir-oai-pmh-openapi.yml
  format: yaml
  label: Kyushu University Institutional Repository (QIR) OAI-PMH
  slug: qir-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyushu/refs/heads/main/openapi/kyushu-qir-oai-pmh-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Kyushu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kyushu University declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Kyushu University
provider_slug: kyushu
scheme_count: 6
schemes:
- description: Fully anonymous. Identify, ListMetadataFormats, ListSets, ListIdentifiers, ListRecords and GetRecord were all answered with no Authorization header, cookie or API key, and no registration of any kind. There are no rate-limit headers on the response; the only documented ceiling is 500 records per list response, paged with resumptionToken.
  endpoint: https://catalog.lib.kyushu-u.ac.jp/mmd/mmd_api/oai-pmh/
  evidence: GET ?verb=Identify -> HTTP 200, valid OAI-PMH XML, no auth challenge.
  name: none
  surface: QIR OAI-PMH (x-operator institution)
  type: none
- description: 'Quarterly full-metadata TSV exports, published through the Handle system under the university''s own 2324 prefix. Anonymous download, no account, no terms acceptance gate. Metadata is CC0 1.0 with one carve-out: QIR abstracts carry no licence grant.'
  endpoint: https://hdl.handle.net/2324/6625737
  evidence: GET https://hdl.handle.net/2324/6625737 -> HTTP 200 landing page for the download.
  name: none
  surface: QIR bulk metadata TSV via Handle (x-operator institution)
  type: none
- description: Kyushu University's own SAML 2.0 IdP, entityID https://idp.kyushu-u.ac.jp/idp/shibboleth, scope kyushu-u.ac.jp, registered in GakuNin since 2011-02-18 and exported to eduGAIN. Declares SingleSignOnService over HTTP-POST, HTTP-Redirect and the Shibboleth 1.0 AuthnRequest profile, and SingleLogoutService over HTTP-POST and HTTP-Redirect with asynchronous SLO support. This authenticates humans into federated services; it is not a machine credential for an API.
  endpoint: https://idp.kyushu-u.ac.jp/idp/profile/SAML2/Redirect/SSO
  evidence: Confirmed inside the 5,653,150-byte GakuNin aggregate metadata (HTTP 200) and independently in the eduGAIN technical API, which reports registrationAuthority https://www.gakunin.jp and registrationInstant 2011-02-18T07:27:49Z. The IdP's own metadata URL https://idp.kyushu-u.ac.jp/idp/shibboleth returns HTTP 200 but a 115-byte Shibboleth error string ("/opt/shibboleth-idp/metadata/idp-metadata.xml そのようなファイルやディレクトリはありません"), so the federation aggregate is the only usable source for this entity — a real, small misconfiguration on the institution's side, recorded rather than glossed.
  name: saml
  surface: GakuNin Shibboleth Identity Provider (x-operator federation)
  type: saml2
  x-anti-pattern: A live 200 that carries a filesystem error string is a soft failure. Anything that grades this endpoint on status code alone will credit metadata that is not being served.
- description: 'Two further GakuNin entities are Kyushu University''s own service providers rather than its IdP: ShareAid, the shared-use research equipment and facility reservation portal (reservation.shareaid.kyushu-u.ac.jp, HTTP 200 live), and a REDCap research-data-capture instance at zk1.med.kyushu-u.ac.jp. Both declare AssertionConsumerService endpoints over HTTP-POST, POST-SimpleSign, HTTP-Artifact and the SAML 1.0 profiles. They consume the federation; they do not expose a public API.'
  endpoint: https://reservation.shareaid.kyushu-u.ac.jp/shibboleth-sp
  evidence: Both EntityDescriptors present in the GakuNin aggregate metadata, OrganizationName "Kyushu University / 九州大学".
  name: none
  surface: Institution-operated SAML service providers (x-operator federation)
  type: none
- description: The Genkai research computing system exposes a user-application portal, a reservation portal and an Open OnDemand instance, all on hpc.kyushu-u.ac.jp. All three answered HTTP 200 with a login surface. Access is granted through an application and fee process run by the Research Institute for Information Technology, not by issuing API credentials; no token format, scope list or programmatic interface is published.
  endpoint: https://genkai-portal.hpc.kyushu-u.ac.jp/user-portal/
  evidence: genkai-portal 200 (3,348 bytes), genkai-ood 200 (6,907 bytes), genkai-reserve 200 (7,475 bytes) — all login walls.
  name: unknown
  surface: Genkai supercomputer portals (x-operator institution)
  type: unknown
- description: Kyushu University's Pure tenant serves a live OpenAPI at /ws/api/openapi.json. It is titled "Pure API", version 5.36.2-1, contact pure-support@elsevier.com, with a relative server block of /ws/api and 827 paths. That is Elsevier's contract running under the university's name, and it is deliberately NOT saved into this repository. Its authentication scheme is Elsevier's to document, not Kyushu's.
  endpoint: https://kyushu-u.elsevierpure.com/ws/api
  evidence: GET /ws/api/openapi.json -> HTTP 200, 360,304 bytes, info.title "Pure API", info.contact.email pure-support@elsevier.com.
  name: oauth2
  surface: Elsevier Pure research portal (x-operator tenant — NOT the institution's contract)
  type: oauth2
slug: kyushu-authentication
source_filename: kyushu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nx-derived-from: live probe of the endpoints listed in source[], run 2026-09-01\nx-source-url: https://catalog.lib.kyushu-u.ac.jp/mmd/mmd_api/oai-pmh/\nsource:\n- https://catalog.lib.kyushu-u.ac.jp/mmd/mmd_api/oai-pmh/\n- https://hdl.handle.net/2324/6625737\n- https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n- https://genkai-portal.hpc.kyushu-u.ac.jp/user-portal/\n- https://kyushu-u.elsevierpure.com/ws/api\nnote: >-\n  Kyushu University issues no API credentials to the public. There is no developer portal, no key\n  request form, no OAuth client registration and no machine-readable terms of use for any surface\n  found in this run. The one place the university runs real credential infrastructure is SAML — its\n  own GakuNin Shibboleth Identity Provider — and that authenticates people into federated services,\n  not callers into an API. Everything below was exercised anonymously on 2026-09-01.\nschemes:\n- name: none\n  type:\
  \ none\n  surface: QIR OAI-PMH (x-operator institution)\n  endpoint: https://catalog.lib.kyushu-u.ac.jp/mmd/mmd_api/oai-pmh/\n  description: >-\n    Fully anonymous. Identify, ListMetadataFormats, ListSets, ListIdentifiers, ListRecords and\n    GetRecord were all answered with no Authorization header, cookie or API key, and no\n    registration of any kind. There are no rate-limit headers on the response; the only documented\n    ceiling is 500 records per list response, paged with resumptionToken.\n  evidence: 'GET ?verb=Identify -> HTTP 200, valid OAI-PMH XML, no auth challenge.'\n- name: none\n  type: none\n  surface: QIR bulk metadata TSV via Handle (x-operator institution)\n  endpoint: https://hdl.handle.net/2324/6625737\n  description: >-\n    Quarterly full-metadata TSV exports, published through the Handle system under the university's\n    own 2324 prefix. Anonymous download, no account, no terms acceptance gate. Metadata is CC0 1.0\n    with one carve-out: QIR abstracts carry\
  \ no licence grant.\n  evidence: 'GET https://hdl.handle.net/2324/6625737 -> HTTP 200 landing page for the download.'\n- name: saml\n  type: saml2\n  surface: GakuNin Shibboleth Identity Provider (x-operator federation)\n  endpoint: https://idp.kyushu-u.ac.jp/idp/profile/SAML2/Redirect/SSO\n  description: >-\n    Kyushu University's own SAML 2.0 IdP, entityID https://idp.kyushu-u.ac.jp/idp/shibboleth,\n    scope kyushu-u.ac.jp, registered in GakuNin since 2011-02-18 and exported to eduGAIN. Declares\n    SingleSignOnService over HTTP-POST, HTTP-Redirect and the Shibboleth 1.0 AuthnRequest profile,\n    and SingleLogoutService over HTTP-POST and HTTP-Redirect with asynchronous SLO support. This\n    authenticates humans into federated services; it is not a machine credential for an API.\n  evidence: >-\n    Confirmed inside the 5,653,150-byte GakuNin aggregate metadata (HTTP 200) and independently in\n    the eduGAIN technical API, which reports registrationAuthority https://www.gakunin.jp\
  \ and\n    registrationInstant 2011-02-18T07:27:49Z. The IdP's own metadata URL\n    https://idp.kyushu-u.ac.jp/idp/shibboleth returns HTTP 200 but a 115-byte Shibboleth error\n    string (\"/opt/shibboleth-idp/metadata/idp-metadata.xml そのようなファイルやディレクトリはありません\"),\n    so the federation aggregate is the only usable source for this entity — a real, small\n    misconfiguration on the institution's side, recorded rather than glossed.\n  x-anti-pattern: >-\n    A live 200 that carries a filesystem error string is a soft failure. Anything that grades this\n    endpoint on status code alone will credit metadata that is not being served.\n- name: none\n  type: none\n  surface: Institution-operated SAML service providers (x-operator federation)\n  endpoint: https://reservation.shareaid.kyushu-u.ac.jp/shibboleth-sp\n  description: >-\n    Two further GakuNin entities are Kyushu University's own service providers rather than its IdP:\n    ShareAid, the shared-use research equipment and facility reservation\
  \ portal\n    (reservation.shareaid.kyushu-u.ac.jp, HTTP 200 live), and a REDCap research-data-capture\n    instance at zk1.med.kyushu-u.ac.jp. Both declare AssertionConsumerService endpoints over\n    HTTP-POST, POST-SimpleSign, HTTP-Artifact and the SAML 1.0 profiles. They consume the\n    federation; they do not expose a public API.\n  evidence: 'Both EntityDescriptors present in the GakuNin aggregate metadata, OrganizationName \"Kyushu University / 九州大学\".'\n- name: unknown\n  type: unknown\n  surface: Genkai supercomputer portals (x-operator institution)\n  endpoint: https://genkai-portal.hpc.kyushu-u.ac.jp/user-portal/\n  description: >-\n    The Genkai research computing system exposes a user-application portal, a reservation portal\n    and an Open OnDemand instance, all on hpc.kyushu-u.ac.jp. All three answered HTTP 200 with a\n    login surface. Access is granted through an application and fee process run by the Research\n    Institute for Information Technology, not by issuing\
  \ API credentials; no token format, scope\n    list or programmatic interface is published.\n  evidence: 'genkai-portal 200 (3,348 bytes), genkai-ood 200 (6,907 bytes), genkai-reserve 200 (7,475 bytes) — all login walls.'\n- name: oauth2\n  type: oauth2\n  surface: Elsevier Pure research portal (x-operator tenant — NOT the institution's contract)\n  endpoint: https://kyushu-u.elsevierpure.com/ws/api\n  description: >-\n    Kyushu University's Pure tenant serves a live OpenAPI at /ws/api/openapi.json. It is titled\n    \"Pure API\", version 5.36.2-1, contact pure-support@elsevier.com, with a relative server block\n    of /ws/api and 827 paths. That is Elsevier's contract running under the university's name, and\n    it is deliberately NOT saved into this repository. Its authentication scheme is Elsevier's to\n    document, not Kyushu's.\n  evidence: 'GET /ws/api/openapi.json -> HTTP 200, 360,304 bytes, info.title \"Pure API\", info.contact.email pure-support@elsevier.com.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyushu/refs/heads/main/authentication/kyushu-authentication.yml
summary_line: 6 schemes
tags:
- University
- Higher Education
- Education
- Research
- Japan
- National University
- Public Research University
- Institutional Repository
- Research Data
- Identity Federation
- Library
- Course Catalog
- Open Access
- OAI-PMH
- Metadata
- Research Computing
---
