---
api_key_in: []
api_specs:
- filename: obie-opendata-openapi.json
  format: json
  label: Skipton Open Banking Open Data API (OBIE Standard)
  slug: skipton-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/obie-opendata-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Skipton Building Society Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skipton Building Society declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Skipton Building Society
provider_slug: skipton-building-society
scheme_count: 0
schemes: []
slug: skipton-building-society-authentication
source_filename: skipton-building-society-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/obie-opendata-openapi.json + review.yml authModel\nnote: >-\n  Derived from the shared OBIE standard the apis[] entries represent; Skipton\n  publishes no proprietary developer platform, so this is the standard auth model,\n  unverified for Skipton (see review.yml).\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\nsurfaces:\n- surface: Open Data (OBIE Open Data standard)\n  spec: openapi/obie-opendata-openapi.json\n  model: none\n  authenticated: false\n  detail: >-\n    The Open Data specification declares no securityDefinitions. Open Data\n    (branches, ATMs, product reference data) is public and unauthenticated by\n    design.\n- surface: Read/Write AIS/PIS/CBPII (OBIE Read/Write standard)\n  spec: null\n  model: fapi-oauth2-oidc-mtls\n  authenticated: true\n  standard_only: true\n  detail: >-\n    The OBIE Read/Write standard mandates FAPI-grade security: OAuth2 authorization\n    code flow, OpenID\
  \ Connect, mutual-TLS with OBIE/eIDAS certificates, and PSD2\n    strong customer authentication. No Skipton Read/Write specification was found;\n    this reflects the standard, not a confirmed Skipton surface.\n  reference: https://openbankinguk.github.io/read-write-api-site3/\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/authentication/skipton-building-society-authentication.yml
summary_line: 0 schemes
tags:
- Financial-Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Mortgages
- Savings
- Account Information
- Payments
---
