---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Nagoya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nagoya University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Nagoya University
provider_slug: nagoya
scheme_count: 0
schemes: []
slug: nagoya-authentication
source_filename: nagoya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes of Nagoya University identity hosts and service pages on 2026-09-01, plus the GakuNin\n  SAML metadata aggregate at https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml.\nnote: >-\n  Nagoya University publishes no API key, OAuth client registration or token endpoint of any kind.\n  This file records the authentication surfaces it DOES operate — a federated SAML identity provider\n  and a campus SSO — and states plainly which surfaces are open and which are closed. Nothing here\n  is a developer credential path; do not read it as one.\nsummary: >-\n  The only machine-readable authentication artifact Nagoya University publishes is its Shibboleth\n  SAML 2.0 identity provider metadata, distributed through the GakuNin federation aggregate. The one\n  institution-operated data surface that is programmatically reachable — the ERG Science Center\n  archive — requires no authentication at all for its open directories.\
  \ The one repository surface —\n  OAI-PMH on the NII WEKO3 tenant — is keyless and open by protocol.\nmechanisms:\n- id: shibboleth-saml\n  type: saml2\n  operator: institution\n  public: true\n  description: >-\n    Institution-operated Shibboleth IdP. entityID https://shib.nagoya-u.ac.jp/idp/shibboleth,\n    scope nagoya-u.ac.jp, registered with GakuNin on 2014-04-30. SingleSignOnService endpoints:\n    /idp/profile/Shibboleth/SSO (Shibboleth 1.0), /idp/profile/SAML2/POST/SSO and\n    /idp/profile/SAML2/Redirect/SSO. An AttributeAuthorityDescriptor role is present. Metadata is\n    obtained from the federation aggregate, not from a per-entity MDQ service — GakuNin publishes a\n    single signed aggregate rather than an mdq endpoint.\n  metadata: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n  endpoint: https://shib.nagoya-u.ac.jp/idp/profile/SAML2/Redirect/SSO\n  evidence:\n  - url: https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\n    status: 200\n  - url: https://shib.nagoya-u.ac.jp/idp/profile/SAML2/Redirect/SSO\n\
  \    status: 500\n  - url: https://icts.nagoya-u.ac.jp/ja/services/gakunin/\n    status: 200\n- id: thers-account-cas\n  type: sso\n  operator: institution\n  public: false\n  description: >-\n    THERS 機構アカウント (Tokai National Higher Education and Research System integrated account) and\n    NU ID, fronted by a CAS single sign-on with multi-factor authentication that the major campus\n    information systems were migrated onto. Human login only; no documented programmatic interface,\n    no client registration, no token endpoint.\n  evidence:\n  - url: https://icts.nagoya-u.ac.jp/en/services/nuid/\n    status: 200\n  - url: https://icts.nagoya-u.ac.jp/ja/services/nuid/CAS/\n    status: 200\n  - url: https://portal.nagoya-u.ac.jp/\n    status: 200\n- id: anonymous-oai\n  type: none\n  operator: tenant\n  public: true\n  description: >-\n    The NAGOYA Repository OAI-PMH interface is keyless and unauthenticated, as the protocol requires.\n    It does content-negotiate on User-Agent at the\
  \ nginx layer: a browser User-Agent gets 406 Not\n    Acceptable, a default client gets 200 XML.\n  endpoint: https://nagoya.repo.nii.ac.jp/oai\n  evidence:\n  - url: https://nagoya.repo.nii.ac.jp/oai?verb=Identify\n    status: 200\n- id: anonymous-ergsc\n  type: none\n  operator: institution\n  public: true\n  description: >-\n    The ERG Science Center open data directories under /data/ergsc/ are served without\n    authentication. Adjacent paths are closed and that boundary was probed, not assumed:\n    /erg_socware/bleeding_edge/ returns 401 (Basic auth for working-group software), /data/ returns\n    403, and the ERG Web Analysis Tool at /ergwat4/login.cgi is a login.\n  endpoint: https://ergsc.isee.nagoya-u.ac.jp/data/ergsc/\n  evidence:\n  - url: https://ergsc.isee.nagoya-u.ac.jp/data/ergsc/\n    status: 200\n  - url: https://ergsc.isee.nagoya-u.ac.jp/data/\n    status: 403\n  - url: https://ergsc.isee.nagoya-u.ac.jp/erg_socware/bleeding_edge/\n    status: 401\nabsent:\n- api-keys\n\
  - oauth2\n- openid-connect\n- client-credentials\n- personal-access-tokens\n- dynamic-client-registration\n- protected-resource-metadata\nabsent_evidence:\n- url: https://www.nagoya-u.ac.jp/.well-known/security.txt\n  status: 404\n- url: https://www.nagoya-u.ac.jp/llms.txt\n  status: 404\n- url: https://developer.nagoya-u.ac.jp/\n  status: 0\n- url: https://api.nagoya-u.ac.jp/\n  status: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nagoya/refs/heads/main/authentication/nagoya-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Japan
- Designated National University
- Research
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- Shibboleth
- Research Data
- Research Computing
---
