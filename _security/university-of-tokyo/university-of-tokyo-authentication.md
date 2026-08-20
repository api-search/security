---
api_key_in: []
api_specs:
- filename: university-of-tokyo-archives-portal-openapi.yml
  format: yaml
  label: UTokyo Academic Assets Archives Portal API
  slug: archives-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-archives-portal-openapi.yml
- filename: university-of-tokyo-archives-portal-openapi.yml
  format: yaml
  label: UTokyo IIIF Presentation and Image APIs
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-archives-portal-openapi.yml
- filename: university-of-tokyo-oai-pmh-openapi.yml
  format: yaml
  label: UTokyo OAI-PMH Metadata Harvesting
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-oai-pmh-openapi.yml
- filename: university-of-tokyo-repository-records-openapi.yml
  format: yaml
  label: UTokyo Repository Records API
  slug: repository-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/openapi/university-of-tokyo-repository-records-openapi.yml
auth_types:
- none
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Tokyo Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Tokyo secures its APIs with none and saml2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Tokyo
provider_slug: university-of-tokyo
scheme_count: 2
schemes:
- applies_to:
  - openapi/university-of-tokyo-oai-pmh-openapi.yml
  - openapi/university-of-tokyo-repository-records-openapi.yml
  - openapi/university-of-tokyo-archives-portal-openapi.yml
  evidence: All OAI-PMH verbs, all /api/records/ requests, all IIIF manifest and info.json requests and all item _format requests returned HTTP 200 with no Authorization header and no cookie. The library documentation states no API key is required.
  name: none
  type: none
- entities:
  - contact: systemshien.adm@gs.mail.u-tokyo.ac.jp
    display_name_en: The University of Tokyo
    display_name_ja: 東京大学
    entity_id: https://gidp.adm.u-tokyo.ac.jp/idp/shibboleth
    role: IdentityProvider
    scope: u-tokyo.ac.jp
    sso_endpoints:
    - https://gidp.adm.u-tokyo.ac.jp/idp/profile/SAML2/Redirect/SSO
    - https://gidp.adm.u-tokyo.ac.jp/idp/profile/SAML2/POST/SSO
    - https://gidp.adm.u-tokyo.ac.jp/idp/profile/Shibboleth/SSO
  - contact: kagra-idp-contact@icrr.u-tokyo.ac.jp
    display_name_en: KAGRA
    entity_id: https://shibbi.pki.itc.u-tokyo.ac.jp/idp/shibboleth
    note: Serves KAGRA, the gravitational-wave observatory operated by the Institute for Cosmic Ray Research. Institution-operated, research-collaboration scoped.
    organization_en: The University of Tokyo
    role: IdentityProvider
    sso_endpoints:
    - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/SAML2/Redirect/SSO
    - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/SAML2/POST/SSO
    - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/Shibboleth/SSO
  - contact: joho.s@gs.mail.u-tokyo.ac.jp
    display_name_en: STEP10 course registration system
    display_name_ja: STEP10聴講申請システム
    entity_id: https://step10.adm.s.u-tokyo.ac.jp/shibboleth-sp
    note: A course-registration service consuming federated identity — the closest thing to a registrar surface the university exposes in a machine-readable form, and it is exposed as an SP entity, not as an API.
    role: ServiceProvider
  evidence: 650 EntityDescriptors in the GakuNin aggregate; exactly 3 carry an entityID under u-tokyo.ac.jp. All three declare mdrpi:registrationAuthority https://www.gakunin.jp and Organization Name "The University of Tokyo" / 東京大学.
  federation: GakuNin (学術認証フェデレーション), registrationAuthority https://www.gakunin.jp
  federation_operator: National Institute of Informatics (NII)
  local_copy: examples/university-of-tokyo-gakunin-saml-metadata.xml
  metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml
  name: GakuNin SAML 2.0 federated single sign-on
  operator: institution
  type: saml2
slug: university-of-tokyo-authentication
source_filename: university-of-tokyo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource:\n  - https://repository.dl.itc.u-tokyo.ac.jp/oai?verb=Identify\n  - https://repository.dl.itc.u-tokyo.ac.jp/api/records/\n  - https://da.dl.itc.u-tokyo.ac.jp/portal/help/api\n  - https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n  - https://utol.ecc.u-tokyo.ac.jp/\n  - https://wisteria-www.cc.u-tokyo.ac.jp/cgi-bin/hpcportal.en/index.cgi\nsummary:\n  types: [none, saml2]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The University of Tokyo's public machine-readable surfaces require no credential at all —\n    there is no API key, no developer registration, no token endpoint and no OAuth server on any\n    institution host. That is not a gap: OAI-PMH, IIIF and the repository records interface are\n    open-access reading surfaces by design and no key exists to issue.\n\n    The university's actual authentication engineering is federated identity, and it is\n    substantial. Two Shibboleth SAML 2.0 Identity Providers\
  \ registered in GakuNin, the Japanese\n    academic access federation operated by the National Institute of Informatics, gate the\n    university's internal and licensed services. That is the institution-operated authentication\n    surface, and it is the one an integrator will actually meet — it just is not reachable as a\n    public API.\nschemes:\n  - name: none\n    type: none\n    applies_to:\n      - openapi/university-of-tokyo-oai-pmh-openapi.yml\n      - openapi/university-of-tokyo-repository-records-openapi.yml\n      - openapi/university-of-tokyo-archives-portal-openapi.yml\n    evidence: >-\n      All OAI-PMH verbs, all /api/records/ requests, all IIIF manifest and info.json requests and\n      all item _format requests returned HTTP 200 with no Authorization header and no cookie. The\n      library documentation states no API key is required.\n  - name: GakuNin SAML 2.0 federated single sign-on\n    type: saml2\n    operator: institution\n    federation: GakuNin (学術認証フェデレーション),\
  \ registrationAuthority https://www.gakunin.jp\n    federation_operator: National Institute of Informatics (NII)\n    entities:\n      - entity_id: https://gidp.adm.u-tokyo.ac.jp/idp/shibboleth\n        role: IdentityProvider\n        display_name_en: The University of Tokyo\n        display_name_ja: 東京大学\n        scope: u-tokyo.ac.jp\n        sso_endpoints:\n          - https://gidp.adm.u-tokyo.ac.jp/idp/profile/SAML2/Redirect/SSO\n          - https://gidp.adm.u-tokyo.ac.jp/idp/profile/SAML2/POST/SSO\n          - https://gidp.adm.u-tokyo.ac.jp/idp/profile/Shibboleth/SSO\n        contact: systemshien.adm@gs.mail.u-tokyo.ac.jp\n      - entity_id: https://shibbi.pki.itc.u-tokyo.ac.jp/idp/shibboleth\n        role: IdentityProvider\n        display_name_en: KAGRA\n        organization_en: The University of Tokyo\n        sso_endpoints:\n          - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/SAML2/Redirect/SSO\n          - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/SAML2/POST/SSO\n\
  \          - https://shibbi.pki.itc.u-tokyo.ac.jp/idp/profile/Shibboleth/SSO\n        contact: kagra-idp-contact@icrr.u-tokyo.ac.jp\n        note: >-\n          Serves KAGRA, the gravitational-wave observatory operated by the Institute for Cosmic\n          Ray Research. Institution-operated, research-collaboration scoped.\n      - entity_id: https://step10.adm.s.u-tokyo.ac.jp/shibboleth-sp\n        role: ServiceProvider\n        display_name_en: STEP10 course registration system\n        display_name_ja: STEP10聴講申請システム\n        contact: joho.s@gs.mail.u-tokyo.ac.jp\n        note: >-\n          A course-registration service consuming federated identity — the closest thing to a\n          registrar surface the university exposes in a machine-readable form, and it is exposed\n          as an SP entity, not as an API.\n    metadata_source: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n    local_copy: examples/university-of-tokyo-gakunin-saml-metadata.xml\n    evidence: >-\n   \
  \   650 EntityDescriptors in the GakuNin aggregate; exactly 3 carry an entityID under\n      u-tokyo.ac.jp. All three declare mdrpi:registrationAuthority https://www.gakunin.jp and\n      Organization Name \"The University of Tokyo\" / 東京大学.\ngated_surfaces:\n  - name: UTOL — University of Tokyo Learning Management System\n    url: https://utol.ecc.u-tokyo.ac.jp/\n    status: 200 (redirects to /login)\n    operator: institution\n    note: >-\n      The university's own LMS, self-hosted on u-tokyo.ac.jp (the former ITC-LMS hostname\n      itc-lms.ecc.u-tokyo.ac.jp resolves to the same login). Institutional credentials only. No\n      public LTI configuration, no public API, no developer documentation.\n  - name: HPC Portal (Wisteria / Miyabi / Information Technology Center)\n    url: https://wisteria-www.cc.u-tokyo.ac.jp/cgi-bin/hpcportal.en/index.cgi\n    status: 200\n    operator: institution\n    note: >-\n      Allocation and job portal for the Information Technology Center's supercomputers.\
  \ Reachable\n      and English-language, but every function behind an account. No service-catalog API is\n      published.\nno_vendor_tenancy_found: true\ntenancy_evidence: >-\n  Probed for the vendor tenancies that dominate this cohort. u-tokyo.figshare.com and\n  utokyo.figshare.com return HTTP 202 with a zero-byte body (Figshare's unknown-tenant\n  response). utokyo.pure.elsevier.com 301s to utokyo.elsevierpure.com, which does not resolve.\n  utokyo.instructure.com returns HTTP 404. utokyo.dataverse.harvard.edu and dataverse.u-tokyo.ac.jp\n  do not resolve. No Figshare, Pure, Symplectic, Dataverse or Canvas tenancy could be\n  substantiated for this institution.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-tokyo/refs/heads/main/authentication/university-of-tokyo-authentication.yml
summary_line: none/saml2 · 2 schemes
tags:
- University
- Higher Education
- Education
- Japan
- Public Research University
- Research Data
- Research Repository
- Library
- Digital Archives
- Identity Federation
- IIIF
- OAI-PMH
- Open Access
- Metadata
---
