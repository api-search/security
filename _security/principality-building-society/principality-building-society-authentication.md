---
api_key_in: []
api_specs:
- filename: obie-open-data-swagger.json
  format: json
  label: OBIE Open Data API (Shared Standard - Unverified for Principality)
  slug: obie-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/obie-open-data-swagger.json
auth_types:
- none
description: ''
kind: authentication
layout: security
method: derived
name: Principality Building Society Authentication
name_suffix: Authentication
oauth_flows: []
overview: Principality Building Society secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Principality Building Society
provider_slug: principality-building-society
scheme_count: 0
schemes: []
slug: principality-building-society-authentication
source_filename: principality-building-society-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: derived\nsource: openapi/obie-open-data-swagger.json\nnote: >-\n  Derived from the shared OBIE Open Data API v1.3 reference specification carried\n  in this repo, NOT a Principality-operated endpoint. The Open Data API is public\n  reference data and defines no security schemes. The OBIE Read/Write APIs\n  (AIS/PIS/CBPII) that Principality does NOT operate would, by the standard, use\n  FAPI-secured OAuth2/OIDC + mutual-TLS + PSD2 SCA; that model is documented in\n  the standard only and no Principality authorization server exists.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public_unauthenticated: true\nschemes: []\nstandard_read_write_model:\n  applies_to: OBIE Read/Write AIS/PIS/CBPII (out of scope for Principality)\n  security: FAPI 1.0 Advanced\n  auth: OAuth2 authorization code + OIDC\n  transport: mutual-TLS\n  customer_auth: PSD2 strong customer authentication\n  operated_by_principality: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/authentication/principality-building-society-authentication.yml
summary_line: none · 0 schemes
tags:
- Financial Services
- Banking
- Building Society
- Savings
- Mortgages
- Open Banking
- Open Data
- PSD2
- OBIE
- United Kingdom
- Wales
- Mutual
---
