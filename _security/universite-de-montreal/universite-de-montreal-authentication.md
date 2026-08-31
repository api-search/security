---
api_key_in: []
api_specs:
- filename: universite-de-montreal-sadvr-openapi.yml
  format: yaml
  label: SADVR REST API (Vitrine-Recherche)
  slug: sadvr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/openapi/universite-de-montreal-sadvr-openapi.yml
auth_types: []
description: 'Authentication posture across Université de Montréal''s programmable surfaces. The pattern is the one most research universities show: the institution''s own read-only research metadata is wide open with no key at all, while everything that touches a person''s account sits behind campus SSO — and there is no self-service developer credential anywhere, because there is no developer portal to issue one from.'
kind: authentication
layout: security
method: probed
name: Universite De Montreal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Université de Montréal declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Université de Montréal
provider_slug: universite-de-montreal
scheme_count: 0
schemes: []
slug: universite-de-montreal-authentication
source_filename: universite-de-montreal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Université de Montréal\nproviderId: universite-de-montreal\ngenerated: '2026-08-30'\nmethod: probed\nsource: live probes of the SADVR, Papyrus and Shibboleth surfaces, 2026-08-30\ndescription: >-\n  Authentication posture across Université de Montréal's programmable surfaces. The pattern is\n  the one most research universities show: the institution's own read-only research metadata is\n  wide open with no key at all, while everything that touches a person's account sits behind\n  campus SSO — and there is no self-service developer credential anywhere, because there is no\n  developer portal to issue one from.\nsurfaces:\n- surface: SADVR REST API (Vitrine-Recherche)\n  x-operator: institution\n  scheme: none\n  registration: not-required\n  detail: >-\n    No API key, no token, no Authorization header, no cookie. Fifteen documented routes were\n    called anonymously on 2026-08-30 and all\
  \ returned 200 application/json, including the full\n    /idext/individu extended-record payload. Read-only: the institution's documentation states\n    the API offers only GET.\n  evidence:\n  - url: https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal/ressource/faculte\n    status: 200\n  - url: https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal/idext/individu?faculte=23\n    status: 200\n  risk: >-\n    Unauthenticated access to personal data. The extended and full record services return\n    researcher names, institutional emails, telephone numbers, office locations and biographies\n    with no rate limit and no credential. The API's own `consentement` block is the only control,\n    and it is advisory to the consumer rather than enforced at the edge.\n- surface: PAPYRUS OAI-PMH (institutional repository)\n  x-operator: tenant\n  scheme: none\n  registration: not-required\n  detail: Anonymous harvesting, per the OAI-PMH 2.0 specification. No key.\n  evidence:\n\
  \  - url: https://umontreal.scholaris.ca/server/oai/openaire4?verb=Identify\n    status: 200\n- surface: PAPYRUS DSpace REST (HAL)\n  x-operator: tenant\n  scheme: none-for-read\n  registration: institutional\n  detail: >-\n    The DSpace 8 HAL root at /server/api answers anonymously and advertises the repository's\n    entry points; writes and any restricted item require a DSpace account issued by the library.\n  evidence:\n  - url: https://umontreal.scholaris.ca/server/api\n    status: 200\n- surface: Borealis Dataverse (UdeM collection)\n  x-operator: tenant\n  scheme: api-token\n  registration: institutional\n  detail: >-\n    Public search and collection reads are anonymous. Deposit requires a Dataverse API token\n    issued by Borealis to an authenticated account, which for UdeM researchers is obtained\n    through campus SSO.\n  evidence:\n  - url: https://borealisdata.ca/api/dataverses/montreal\n    status: 200\n- surface: UdeM Shibboleth Identity Provider\n  x-operator: institution\n\
  \  scheme: saml2\n  registration: federation\n  detail: >-\n    This is not an API to authenticate against — it is the institution's authentication\n    infrastructure. Relying parties join by exchanging SAML metadata through the federation, not\n    by signing up. The metadata document is public and unauthenticated; the SSO endpoints\n    themselves reject direct GETs (500 from the Redirect/SSO profile without a valid AuthnRequest).\n  evidence:\n  - url: https://shibboleth.umontreal.ca/idp/shibboleth\n    status: 200\n  - url: https://shibboleth.umontreal.ca/idp/profile/SAML2/Redirect/SSO\n    status: 500\n- surface: api.umontreal.ca\n  x-operator: institution\n  scheme: unknown\n  registration: not-public\n  detail: >-\n    The host resolves and answers, but returns HTTP 400 with an empty body on every path tried\n    anonymously. No documentation on any umontreal.ca surface names it. Treated as an internal\n    gateway, not a published API.\n  evidence:\n  - url: https://api.umontreal.ca/\n\
  \    status: 400\nsummary:\n  self_service_credential: false\n  developer_portal: false\n  oauth2: false\n  api_keys_issued: false\n  campus_sso: shibboleth\nnotes: >-\n  There is no route by which an outside developer can obtain a credential for any Université de\n  Montréal API. What is open is open to everyone anonymously; what is closed is closed to anyone\n  without a UdeM account. Nothing sits in between.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/authentication/universite-de-montreal-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Canada
- Québec
- French Language
- U15
- Public Research University
- Research
- Research Data
- Research Expertise
- Identity Federation
- Institutional Repository
- Library
- Open Access
- OAI-PMH
- Shibboleth
- SAML
---
