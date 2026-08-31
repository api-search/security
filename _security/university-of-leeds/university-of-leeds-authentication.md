---
api_key_in: []
api_specs:
- filename: university-of-leeds-research-data-oai-pmh-openapi.yml
  format: yaml
  label: Research Data Leeds Repository (OAI-PMH)
  slug: research-data-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-research-data-oai-pmh-openapi.yml
- filename: university-of-leeds-digital-library-openapi.yml
  format: yaml
  label: Leeds Digital Library (OAI-PMH and OpenSearch)
  slug: digital-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-digital-library-openapi.yml
- filename: university-of-leeds-spacefinder-openapi.yml
  format: yaml
  label: Spacefinder Campus Space Data
  slug: spacefinder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-spacefinder-openapi.yml
- filename: university-of-leeds-library-floorplans-iiif-openapi.yml
  format: yaml
  label: Library Floor Plans IIIF Image API
  slug: library-floorplans-iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/openapi/university-of-leeds-library-floorplans-iiif-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: University Of Leeds Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Leeds declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Leeds
provider_slug: university-of-leeds
scheme_count: 0
schemes: []
slug: university-of-leeds-authentication
source_filename: university-of-leeds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "authentication: '0.1'\nprovider: university-of-leeds\ngenerated: '2026-08-30'\nmethod: derived\nevidence_method: probed\nprobed: '2026-08-30'\nsource: >-\n  Established by issuing unauthenticated requests to each institution-operated surface on 2026-08-30\n  and observing that all returned complete payloads at HTTP 200 with no credential of any kind.\nx-operator: institution\nsummary: >-\n  Every institution-operated surface the University of Leeds exposes is fully anonymous. There is no\n  registration, no key issuance, no OAuth flow, no rate-limit header and no developer account. This\n  is a genuine open-access posture, not an undocumented one — but it also means there is no\n  onboarding path, no way to identify a caller, and no contact route for a consumer with a problem.\nsurfaces:\n  - surface: Spacefinder space data\n    baseURL: https://spacefinder.leeds.ac.uk/spaces.json\n    scheme: none\n    verified: '2026-08-30'\n    evidence: 'GET with no headers returned HTTP\
  \ 200 and 137,649 bytes of JSON.'\n  - surface: Research Data Leeds Repository OAI-PMH\n    baseURL: https://archive.researchdata.leeds.ac.uk/cgi/oai2\n    scheme: none\n    verified: '2026-08-30'\n    evidence: 'verb=Identify and verb=ListIdentifiers both returned HTTP 200 unauthenticated.'\n  - surface: Leeds Digital Library OAI-PMH / OpenSearch\n    baseURL: https://digital.library.leeds.ac.uk/cgi/oai2\n    scheme: none\n    verified: '2026-08-30'\n    evidence: 'verb=Identify returned HTTP 200 unauthenticated.'\n  - surface: Library floor plans IIIF Image API\n    baseURL: https://floorplans.library.leeds.ac.uk/assets/iiif\n    scheme: none\n    verified: '2026-08-30'\n    evidence: 'info.json and a derivative tile both returned HTTP 200 unauthenticated.'\nnot_applicable:\n  - surface: Library Search (Ex Libris Alma / Primo)\n    x-operator: tenant\n    detail: >-\n      Programmatic access runs through Ex Libris' Alma and Primo REST APIs and requires an\n      institution-issued key\
  \ obtained from Ex Libris, not from Leeds. The authentication model is\n      the vendor's, and it is documented on the vendor's developer network — not here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/authentication/university-of-leeds-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Research Repository
- Libraries
- Open Data
- OAI-PMH
- IIIF
- Research Computing
- Digital Collections
---
