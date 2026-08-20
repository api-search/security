---
api_key_in:
- header
api_specs:
- filename: placer-account-info-api-openapi.yml
  format: yaml
  label: Placer Account Info API
  slug: placer-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-account-info-api-openapi.yml
- filename: placer-loyalty-reports-api-openapi.yml
  format: yaml
  label: Placer Loyalty Reports API
  slug: placer-loyalty-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-loyalty-reports-api-openapi.yml
- filename: placer-manage-pois-api-openapi.yml
  format: yaml
  label: Placer Manage POIs API
  slug: placer-manage-pois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-manage-pois-api-openapi.yml
- filename: placer-ranking-reports-api-openapi.yml
  format: yaml
  label: Placer Ranking Reports API
  slug: placer-ranking-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-ranking-reports-api-openapi.yml
- filename: placer-retail-sales-reports-api-openapi.yml
  format: yaml
  label: Placer Retail Sales Reports API
  slug: placer-retail-sales-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-retail-sales-reports-api-openapi.yml
- filename: placer-trade-area-reports-api-openapi.yml
  format: yaml
  label: Placer Trade Area Reports API
  slug: placer-trade-area-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-trade-area-reports-api-openapi.yml
- filename: placer-visitor-journey-reports-api-openapi.yml
  format: yaml
  label: Placer Visitor Journey Reports API
  slug: placer-visitor-journey-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-visitor-journey-reports-api-openapi.yml
- filename: placer-visits-reports-api-openapi.yml
  format: yaml
  label: Placer Visits Reports API
  slug: placer-visits-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/openapi/placer-visits-reports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Placer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Placer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Placer
provider_slug: placer
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/placer-papi-openapi.json
  type: apiKey
slug: placer-authentication
source_filename: placer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/placer-papi-openapi.json\ndocs: https://docs.placer.ai/reference/getting-started\nnotes: >-\n  The Placer API (PAPI) authenticates every request with a static API key\n  passed in the `x-api-key` HTTP header. Keys are issued/managed by Placer\n  (contact a CSM or the MyZone Support Portal). A missing or invalid key\n  returns HTTP 403 (\"Forbidden, wrong or missing API Key\").\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/placer-papi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placer/refs/heads/main/authentication/placer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Location Analytics
- Foot Traffic
- Geospatial
- Retail Analytics
- Real-Estate
- Consumer Insights
- Data
---
