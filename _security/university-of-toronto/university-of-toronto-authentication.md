---
api_key_in: []
api_specs:
- filename: university-of-toronto-timetable-builder-openapi.yml
  format: yaml
  label: Timetable Builder API
  slug: ttb-course-timetable
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/openapi/university-of-toronto-timetable-builder-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Toronto Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Toronto declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Toronto
provider_slug: university-of-toronto
scheme_count: 0
schemes: []
slug: university-of-toronto-authentication
source_filename: university-of-toronto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of https://api.easi.utoronto.ca/ttb and\n  https://idpz.utorauth.utoronto.ca/idp/shibboleth on 2026-08-19, plus the SAML 2.0 metadata that\n  endpoint serves.\nx-operator: institution\nsummary: >-\n  The University of Toronto operates two entirely separate authentication stories, and neither is a\n  developer-facing one. The public Timetable Builder API requires no credential at all. Everything\n  the University actually gates — ACORN, Quercus, library resources, Microsoft 365 — is gated behind\n  UTORid via a SAML 2.0 Shibboleth identity provider registered in the Canadian Access Federation.\n  There is no OAuth authorization server, no API key issuance, no client registration, and no\n  developer account of any kind.\nsurfaces:\n  - api: university-of-toronto:ttb-course-timetable\n    host: api.easi.utoronto.ca\n    x-operator: institution\n    scheme: none\n    verified: '2026-08-19'\n    evidence:\n\
  \      - url: https://api.easi.utoronto.ca/ttb/reference-data\n        status: 200\n        note: 200 with no Authorization header, no cookie, no API key.\n    browser_restriction:\n      header: 'Access-Control-Allow-Origin: https://ttb.utoronto.ca'\n      note: >-\n        CORS is pinned to the official UI origin, so a browser-based third-party client is blocked\n        while a server-side client is not. This is an origin restriction, not authentication, and it\n        is the only access control observed on the surface.\n  - api: university-of-toronto:utorauth-shibboleth-idp\n    host: idpz.utorauth.utoronto.ca\n    x-operator: institution\n    scheme: SAML 2.0 Web Browser SSO (Shibboleth IdP)\n    entity_id: https://idpz.utorauth.utoronto.ca/shibboleth\n    verified: '2026-08-19'\n    evidence:\n      - url: https://idpz.utorauth.utoronto.ca/idp/shibboleth\n        status: 200\n        note: >-\n          Serves a signed md:EntityDescriptor. Registration authority http://www.canarie.ca\n\
  \          (Canadian Access Federation), registered 2018-09-21.\n    entity_categories:\n      - http://refeds.org/category/research-and-scholarship\n    assurance:\n      - https://refeds.org/sirtfi\n    note: >-\n      This is a federation login endpoint for humans in a browser, not an API authorization server.\n      It is catalogued because it is machine-readable, institution-operated, and the University's\n      only published conformance to an identity standard.\n  - api: university-of-toronto:tspace-dspace-rest\n    host: utoronto.scholaris.ca\n    x-operator: tenant\n    scheme: DSpace 8 authn endpoint (/server/api/authn), vendor-defined\n    verified: '2026-08-19'\n    note: >-\n      The authentication design here is the Scholaris/DSpace platform's, not the University's. Read\n      access to the repository requires no credential.\ngaps:\n  - No OAuth 2.0 or OpenID Connect surface published for third-party developers.\n  - No API key programme, developer registration, or client\
  \ credential issuance.\n  - No published authentication documentation for any institution-operated API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/authentication/university-of-toronto-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Canada
- U15
- Research
- Course Catalog
- Identity Federation
- Research Data
- Institutional Repository
- Library
- Public Research University
---
