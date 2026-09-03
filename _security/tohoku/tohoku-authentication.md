---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Tohoku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tohoku University declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Tohoku University
provider_slug: tohoku
scheme_count: 4
schemes:
- description: Fully anonymous. POST with content-type application/json is answered without any Authorization header, cookie or API key. Introspection is enabled anonymously. Verified with two live domain queries (see examples/).
  endpoint: https://jmorp.megabank.tohoku.ac.jp/api/graphql
  evidence: POST {"query":"{ dataset(limit:1){datasetId} }"} returned HTTP 200 with data and no auth challenge.
  name: none
  surface: jMorp GraphQL (x-operator institution)
  type: none
- description: A logged-in tier exists behind the portal. GET /api/user/profile/ returns HTTP 403 anonymously. No registration flow, scope list or token format is published; controlled-access datasets are flagged in the schema by Dataset.dtaRequired (Data Transfer Agreement required) and are handled as a paperwork process, not as an API scope.
  endpoint: https://jmorp.megabank.tohoku.ac.jp/api/user/profile/
  evidence: GET /api/user/profile/ -> HTTP 403 (anonymous). No public documentation of the login.
  name: session
  surface: jMorp portal account (undocumented)
  type: cookie
- description: OAI-PMH 2.0 harvesting is open and unauthenticated, as the protocol intends. Verb-based GET only. Implemented by NII JAIRO Cloud (WEKO3), not by Tohoku University.
  endpoint: https://tohoku.repo.nii.ac.jp/oai
  evidence: ?verb=Identify and ?verb=ListMetadataFormats both returned HTTP 200 with valid OAI-PMH XML.
  name: none
  surface: TOUR OAI-PMH (x-operator tenant)
  type: none
- description: Tohoku University operates its own SAML 2.0 Identity Provider, registered in GakuNin — the Japanese academic access-management federation run by NII. Scope auth.tohoku.ac.jp; OrganizationName "Tohoku University / 東北大学". The IdP identity and the attribute scope are the university's; the SSO endpoint itself is hosted by SECIOSS (slink.secioss.com), so the operation is outsourced while the entity is theirs. HTTP-Redirect binding for both SingleSignOn and SingleLogout.
  entity_id: https://idp.auth.tohoku.ac.jp/idp/shibboleth
  evidence: 'EntityDescriptor with an IDPSSODescriptor found in the GakuNin aggregate metadata (https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml, HTTP 200, 5.65 MB, fetched 2026-09-01). A second Tohoku University entity is registered as a Service Provider: https://sp.corona-vaccine.hosp.tohoku.ac.jp/shibboleth-sp (Corona Vaccine Reservation System); that host no longer resolves, so the SP entry is stale metadata for a decommissioned service.'
  name: shibboleth-saml
  slo_endpoint: https://slink.secioss.com/saml/saml2/idp/SingleLogoutService.php
  sso_endpoint: https://slink.secioss.com/saml/saml2/idp/SSOService.php/auth.tohoku.ac.jp
  surface: GakuNin identity federation (x-operator federation)
  type: saml2
slug: tohoku-authentication
source_filename: tohoku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nx-derived-from: live probe of the endpoints listed in source[], run 2026-09-01\nx-source-url: https://jmorp.megabank.tohoku.ac.jp/api/graphql\nsource:\n- https://jmorp.megabank.tohoku.ac.jp/api/graphql\n- https://jmorp.megabank.tohoku.ac.jp/api/user/profile/\n- https://tohoku.repo.nii.ac.jp/oai\n- https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml\nnote: >-\n  Tohoku University issues no API credentials to the public. There is no developer portal, no key\n  request form, no OAuth client registration and no documented terms of use for any of its\n  machine-readable surfaces. Every anonymous surface below was exercised on 2026-09-01. The one\n  place where the university does run real credential infrastructure is SAML — its GakuNin\n  Shibboleth IdP — and that authenticates people into federated services, not callers into an API.\nschemes:\n- name: none\n  type: none\n  surface: jMorp GraphQL (x-operator institution)\n  endpoint:\
  \ https://jmorp.megabank.tohoku.ac.jp/api/graphql\n  description: >-\n    Fully anonymous. POST with content-type application/json is answered without any Authorization\n    header, cookie or API key. Introspection is enabled anonymously. Verified with two live domain\n    queries (see examples/).\n  evidence: 'POST {\"query\":\"{ dataset(limit:1){datasetId} }\"} returned HTTP 200 with data and no auth challenge.'\n- name: session\n  type: cookie\n  surface: jMorp portal account (undocumented)\n  endpoint: https://jmorp.megabank.tohoku.ac.jp/api/user/profile/\n  description: >-\n    A logged-in tier exists behind the portal. GET /api/user/profile/ returns HTTP 403 anonymously.\n    No registration flow, scope list or token format is published; controlled-access datasets are\n    flagged in the schema by Dataset.dtaRequired (Data Transfer Agreement required) and are handled\n    as a paperwork process, not as an API scope.\n  evidence: 'GET /api/user/profile/ -> HTTP 403 (anonymous). No\
  \ public documentation of the login.'\n- name: none\n  type: none\n  surface: TOUR OAI-PMH (x-operator tenant)\n  endpoint: https://tohoku.repo.nii.ac.jp/oai\n  description: >-\n    OAI-PMH 2.0 harvesting is open and unauthenticated, as the protocol intends. Verb-based GET\n    only. Implemented by NII JAIRO Cloud (WEKO3), not by Tohoku University.\n  evidence: '?verb=Identify and ?verb=ListMetadataFormats both returned HTTP 200 with valid OAI-PMH XML.'\n- name: shibboleth-saml\n  type: saml2\n  surface: GakuNin identity federation (x-operator federation)\n  entity_id: https://idp.auth.tohoku.ac.jp/idp/shibboleth\n  description: >-\n    Tohoku University operates its own SAML 2.0 Identity Provider, registered in GakuNin — the\n    Japanese academic access-management federation run by NII. Scope auth.tohoku.ac.jp;\n    OrganizationName \"Tohoku University / 東北大学\". The IdP identity and the attribute scope are\n    the university's; the SSO endpoint itself is hosted by SECIOSS (slink.secioss.com),\
  \ so the\n    operation is outsourced while the entity is theirs. HTTP-Redirect binding for both\n    SingleSignOn and SingleLogout.\n  sso_endpoint: https://slink.secioss.com/saml/saml2/idp/SSOService.php/auth.tohoku.ac.jp\n  slo_endpoint: https://slink.secioss.com/saml/saml2/idp/SingleLogoutService.php\n  evidence: >-\n    EntityDescriptor with an IDPSSODescriptor found in the GakuNin aggregate metadata\n    (https://metadata.gakunin.nii.ac.jp/gakunin-metadata.xml, HTTP 200, 5.65 MB, fetched\n    2026-09-01). A second Tohoku University entity is registered as a Service Provider:\n    https://sp.corona-vaccine.hosp.tohoku.ac.jp/shibboleth-sp (Corona Vaccine Reservation System);\n    that host no longer resolves, so the SP entry is stale metadata for a decommissioned service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tohoku/refs/heads/main/authentication/tohoku-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- Japan
- National University
- Public Research University
- Genomics
- Research Data
- Institutional Repository
- Identity Federation
- Course Catalog
- Library
- Open Access
- OAI-PMH
- GraphQL
---
