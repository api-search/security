---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tender-radar-co-uk-buyers-api-openapi.yml
  format: yaml
  label: Tender Radar Buyers API
  slug: tender-radar-co-uk-buyers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-buyers-api-openapi.yml
- filename: tender-radar-co-uk-contracts-api-openapi.yml
  format: yaml
  label: Tender Radar Contracts API
  slug: tender-radar-co-uk-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-contracts-api-openapi.yml
- filename: tender-radar-co-uk-matches-api-openapi.yml
  format: yaml
  label: Tender Radar Matches API
  slug: tender-radar-co-uk-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-matches-api-openapi.yml
- filename: tender-radar-co-uk-renewals-api-openapi.yml
  format: yaml
  label: Tender Radar Renewals API
  slug: tender-radar-co-uk-renewals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-renewals-api-openapi.yml
- filename: tender-radar-co-uk-suppliers-api-openapi.yml
  format: yaml
  label: Tender Radar Suppliers API
  slug: tender-radar-co-uk-suppliers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-suppliers-api-openapi.yml
- filename: tender-radar-co-uk-tenders-api-openapi.yml
  format: yaml
  label: Tender Radar Tenders API
  slug: tender-radar-co-uk-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-radar-co-uk/openapi/tender-radar-co-uk-tenders-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tender Radar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tender Radar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tender Radar
provider_slug: tender-radar-co-uk
scheme_count: 1
schemes:
- description: Your key, which starts tr_.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/tender-radar-co-uk-openapi.json
  type: http
slug: tender-radar-co-uk-authentication
source_filename: tender-radar-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/tender-radar-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Your key, which starts tr_.\n  sources:\n  - openapi/tender-radar-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tender-radar-co-uk/authentication/tender-radar-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Public Sector
- Procurement
- Data Aggregation
- United Kingdom
---
