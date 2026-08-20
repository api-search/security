---
api_key_in: []
api_specs:
- filename: cornell-class-roster-api-openapi.yml
  format: yaml
  label: Cornell Class Roster API
  slug: class-roster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-class-roster-api-openapi.yml
- filename: cornell-library-catalog-api-openapi.yml
  format: yaml
  label: Cornell University Library Catalog Search API
  slug: library-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-library-catalog-api-openapi.yml
- filename: cugir-geospatial-api-openapi.yml
  format: yaml
  label: CUGIR — Cornell University Geospatial Information Repository API
  slug: cugir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cugir-geospatial-api-openapi.yml
auth_types:
- none
- apiKey
- saml
description: ''
kind: authentication
layout: security
method: probed
name: Cornell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cornell University secures its APIs with none, apiKey, and saml across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cornell University
provider_slug: cornell
scheme_count: 6
schemes:
- applies_to: https://classes.cornell.edu/api/2.0
  description: 'The Cornell Class Roster API is public and read-only; no key, token or header is required. Probed 2026-08-19: /config/rosters.json and /search/classes.json both 200 with no credential. Cornell asks clients to stay under one request per second.'
  evidence:
    status: 200
    url: https://classes.cornell.edu/api/2.0/config/rosters.json
  name: ClassRosterPublic
  operator: institution
  type: none
- applies_to: https://catalog.library.cornell.edu
  description: Cornell University Library's Blacklight catalog serves JSON with no credential. The HTML root answers HTTP 202 with an empty body to non-browser clients (a bot challenge); the .json routes are unaffected.
  evidence:
    status: 200
    url: https://catalog.library.cornell.edu/catalog.json?q=cornell&search_field=all_fields
  name: LibraryCatalogPublic
  operator: institution
  type: none
- applies_to: https://cugir.library.cornell.edu
  description: CUGIR's GeoBlacklight JSON routes are open, unauthenticated reads.
  evidence:
    status: 200
    url: https://cugir.library.cornell.edu/catalog.json?q=ithaca
  name: CugirPublic
  operator: institution
  type: none
- applies_to: https://api.ebird.org/v2
  description: 'The eBird API 2.0, run by the Cornell Lab of Ornithology, requires a free API token requested at https://ebird.org/api/keygen. Probed 2026-08-19: an unauthenticated call and a call with an invalid token both return HTTP 403 with an empty body — the surface is gated, not dead.'
  evidence:
    status: 403
    url: https://api.ebird.org/v2/ref/region/list/subnational1/US
  in: header
  name: eBirdApiToken
  operator: institution
  parameter: X-eBirdApiToken
  type: apiKey
- applies_to: https://ecommons.cornell.edu/server/api
  description: eCommons serves DSpace 8.2 REST and OAI-PMH reads without authentication. Deposit and administration authenticate against the DSpace platform, whose auth model is 4Science/DSpace's, not Cornell's.
  evidence:
    status: 200
    url: https://ecommons.cornell.edu/server/api
  name: eCommonsDSpacePublicRead
  operator: tenant
  type: none
- applies_to: https://shibidp.cit.cornell.edu/idp/shibboleth
  description: Cornell's institutional systems federate through its own Shibboleth IdP, published as SAML 2.0 metadata and registered with InCommon/eduGAIN. This is Cornell's own identity surface and the only machine-readable authentication contract the institution itself publishes.
  evidence:
    status: 200
    url: https://shibidp.cit.cornell.edu/idp/shibboleth
  name: ShibbolethSAML
  operator: institution
  type: saml
slug: cornell-authentication
source_filename: cornell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes 2026-08-19 of every surface attributed to Cornell University, plus\n  openapi/cornell-class-roster-api-openapi.yml. Replaces the 2026-07-11 file, which derived an\n  `apiKey in query` scheme from openapi/_original/cornell-codi-events.yaml — the Localist\n  (events.cornell.edu) contract. That was a vendor's auth model recorded as Cornell's.\nprovider: Cornell University\nproviderId: cornell\nsummary:\n  types:\n  - none\n  - apiKey\n  - saml\n  institution_operated_public_apis_requiring_no_auth: 3\nschemes:\n- name: ClassRosterPublic\n  type: none\n  operator: institution\n  applies_to: https://classes.cornell.edu/api/2.0\n  description: >-\n    The Cornell Class Roster API is public and read-only; no key, token or header is required.\n    Probed 2026-08-19: /config/rosters.json and /search/classes.json both 200 with no credential.\n    Cornell asks clients to stay under one request per second.\n  evidence:\n\
  \    url: https://classes.cornell.edu/api/2.0/config/rosters.json\n    status: 200\n- name: LibraryCatalogPublic\n  type: none\n  operator: institution\n  applies_to: https://catalog.library.cornell.edu\n  description: >-\n    Cornell University Library's Blacklight catalog serves JSON with no credential. The HTML root\n    answers HTTP 202 with an empty body to non-browser clients (a bot challenge); the .json routes\n    are unaffected.\n  evidence:\n    url: https://catalog.library.cornell.edu/catalog.json?q=cornell&search_field=all_fields\n    status: 200\n- name: CugirPublic\n  type: none\n  operator: institution\n  applies_to: https://cugir.library.cornell.edu\n  description: CUGIR's GeoBlacklight JSON routes are open, unauthenticated reads.\n  evidence:\n    url: https://cugir.library.cornell.edu/catalog.json?q=ithaca\n    status: 200\n- name: eBirdApiToken\n  type: apiKey\n  in: header\n  parameter: X-eBirdApiToken\n  operator: institution\n  applies_to: https://api.ebird.org/v2\n\
  \  description: >-\n    The eBird API 2.0, run by the Cornell Lab of Ornithology, requires a free API token requested\n    at https://ebird.org/api/keygen. Probed 2026-08-19: an unauthenticated call and a call with an\n    invalid token both return HTTP 403 with an empty body — the surface is gated, not dead.\n  evidence:\n    url: https://api.ebird.org/v2/ref/region/list/subnational1/US\n    status: 403\n- name: eCommonsDSpacePublicRead\n  type: none\n  operator: tenant\n  applies_to: https://ecommons.cornell.edu/server/api\n  description: >-\n    eCommons serves DSpace 8.2 REST and OAI-PMH reads without authentication. Deposit and\n    administration authenticate against the DSpace platform, whose auth model is 4Science/DSpace's,\n    not Cornell's.\n  evidence:\n    url: https://ecommons.cornell.edu/server/api\n    status: 200\n- name: ShibbolethSAML\n  type: saml\n  operator: institution\n  applies_to: https://shibidp.cit.cornell.edu/idp/shibboleth\n  description: >-\n    Cornell's\
  \ institutional systems federate through its own Shibboleth IdP, published as SAML 2.0\n    metadata and registered with InCommon/eduGAIN. This is Cornell's own identity surface and the\n    only machine-readable authentication contract the institution itself publishes.\n  evidence:\n    url: https://shibidp.cit.cornell.edu/idp/shibboleth\n    status: 200\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/authentication/cornell-authentication.yml
summary_line: none/apiKey/saml · 6 schemes
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- Course Catalog
- Library
- Research Data
- Geospatial
- Identity Federation
---
