---
api_key_in: []
api_specs:
- filename: michigan-state-university-record-api-openapi.yml
  format: yaml
  label: MSU Libraries Catalog Record API
  slug: michigan-state-university-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/openapi/michigan-state-university-record-api-openapi.yml
- filename: michigan-state-university-search-api-openapi.yml
  format: yaml
  label: MSU Libraries Catalog Search API
  slug: michigan-state-university-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/openapi/michigan-state-university-search-api-openapi.yml
auth_types: []
description: How authentication works across Michigan State University's institution-operated surfaces. MSU operates no API key programme, no developer registration, and no OAuth authorization server for public API consumers. The public read surfaces are open and unauthenticated; everything else is gated by institutional identity through the university's Shibboleth Identity Provider, which is a federation membership question rather than an API onboarding one.
kind: authentication
layout: security
method: probed
name: Michigan State University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Michigan State University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Michigan State University
provider_slug: michigan-state-university
scheme_count: 0
schemes: []
slug: michigan-state-university-authentication
source_filename: michigan-state-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Michigan State University\nproviderId: michigan-state-university\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://catalog.lib.msu.edu/api/v1/?swagger (live OpenAPI, no securitySchemes declared);\n  https://idp.idm.msu.edu/idp/shibboleth (live SAML 2.0 metadata);\n  live unauthenticated probes of each MSU-operated endpoint, 2026-08-30\ndescription: >-\n  How authentication works across Michigan State University's institution-operated surfaces.\n  MSU operates no API key programme, no developer registration, and no OAuth authorization\n  server for public API consumers. The public read surfaces are open and unauthenticated;\n  everything else is gated by institutional identity through the university's Shibboleth\n  Identity Provider, which is a federation membership question rather than an API onboarding one.\nsurfaces:\n- name: MSU Libraries Catalog REST API (VuFind)\n  baseURL:\
  \ https://catalog.lib.msu.edu/api/v1\n  operator: institution\n  scheme: none\n  registration: not_required\n  evidence:\n  - url: https://catalog.lib.msu.edu/api/v1/search?lookfor=test&limit=1\n    status: 200\n    note: Unauthenticated GET returned a populated SearchResponse envelope.\n  - url: https://catalog.lib.msu.edu/api/v1/?swagger\n    status: 200\n    note: >-\n      The published OpenAPI declares no components.securitySchemes and no security requirement\n      on any of its six operations. The Unauthorized schema exists in components but is\n      unreferenced by any operation response.\n- name: MSU Libraries Catalog OAI-PMH\n  baseURL: https://catalog.lib.msu.edu/OAI/Server\n  operator: institution\n  scheme: none\n  registration: not_required\n  evidence:\n  - url: https://catalog.lib.msu.edu/OAI/Server?verb=Identify\n    status: 200\n- name: MSU Libraries Digital Repository OAI-PMH\n  baseURL: https://d.lib.msu.edu/oai\n  operator: institution\n  scheme: none\n  registration:\
  \ not_required\n  evidence:\n  - url: https://d.lib.msu.edu/oai?verb=Identify\n    status: 200\n- name: MSU Identity Provider\n  baseURL: https://idp.idm.msu.edu/idp/shibboleth\n  operator: institution\n  scheme: saml2\n  registration: federation_membership\n  detail: >-\n    SAML 2.0 / Shibboleth IdP registered in InCommon as urn:mace:incommon:msu.edu. The\n    metadata document itself is public and unauthenticated; obtaining assertions requires\n    a registered service provider and an MSU NetID, i.e. institutional affiliation. This is\n    not a self-service developer credential and cannot be onboarded to from outside.\n  evidence:\n  - url: https://idp.idm.msu.edu/idp/shibboleth\n    status: 200\nnot_available:\n- what: API keys\n  detail: No key issuance, developer account, or application registration surface found on any MSU host.\n- what: OAuth 2.0 authorization server\n  detail: >-\n    MSU's IT documentation describes OAuth 2.0 support for institutionally integrated\n    applications,\
  \ but no public authorization or token endpoint, and no .well-known\n    OAuth or OpenID Connect discovery document, was reachable on an MSU host.\n- what: Administrative / student-record APIs\n  detail: >-\n    Not offered publicly. https://d.lib.msu.edu/api returns 401 with\n    WWW-Authenticate: Basic realm=\"traefik\" — an internal operations endpoint, not a\n    public API with a documented credential path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/authentication/michigan-state-university-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Public Research University
- Land Grant University
- Big Ten
- United States
- Michigan
- Library
- Library Catalog
- Digital Repository
- Metadata
- OAI-PMH
- Identity Federation
- Shibboleth
- Research Computing
---
