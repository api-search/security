---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edinetdb-jp-companies-api-openapi.yml
  format: yaml
  label: edinetdb-jp Companies API
  slug: edinetdb-jp-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-companies-api-openapi.yml
- filename: edinetdb-jp-corp-api-openapi.yml
  format: yaml
  label: edinetdb-jp Corp API
  slug: edinetdb-jp-corp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-corp-api-openapi.yml
- filename: edinetdb-jp-corporate-graph-api-openapi.yml
  format: yaml
  label: edinetdb-jp Corporate Graph API
  slug: edinetdb-jp-corporate-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-corporate-graph-api-openapi.yml
- filename: edinetdb-jp-earnings-api-openapi.yml
  format: yaml
  label: edinetdb-jp Earnings API
  slug: edinetdb-jp-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-earnings-api-openapi.yml
- filename: edinetdb-jp-events-api-openapi.yml
  format: yaml
  label: edinetdb-jp Events API
  slug: edinetdb-jp-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-events-api-openapi.yml
- filename: edinetdb-jp-governance-api-openapi.yml
  format: yaml
  label: edinetdb-jp Governance API
  slug: edinetdb-jp-governance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-governance-api-openapi.yml
- filename: edinetdb-jp-industries-api-openapi.yml
  format: yaml
  label: edinetdb-jp Industries API
  slug: edinetdb-jp-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-industries-api-openapi.yml
- filename: edinetdb-jp-ir-kpis-api-openapi.yml
  format: yaml
  label: edinetdb-jp IR KPIs API
  slug: edinetdb-jp-ir-kpis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-ir-kpis-api-openapi.yml
- filename: edinetdb-jp-ir-pdf-distribution-api-openapi.yml
  format: yaml
  label: edinetdb-jp IR PDF Distribution API
  slug: edinetdb-jp-ir-pdf-distribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-ir-pdf-distribution-api-openapi.yml
- filename: edinetdb-jp-ir-sections-api-openapi.yml
  format: yaml
  label: edinetdb-jp IR Sections API
  slug: edinetdb-jp-ir-sections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-ir-sections-api-openapi.yml
- filename: edinetdb-jp-queries-api-openapi.yml
  format: yaml
  label: edinetdb-jp Queries API
  slug: edinetdb-jp-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-queries-api-openapi.yml
- filename: edinetdb-jp-rankings-api-openapi.yml
  format: yaml
  label: edinetdb-jp Rankings API
  slug: edinetdb-jp-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-rankings-api-openapi.yml
- filename: edinetdb-jp-real-estate-api-openapi.yml
  format: yaml
  label: edinetdb-jp Real Estate API
  slug: edinetdb-jp-real-estate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-real-estate-api-openapi.yml
- filename: edinetdb-jp-screener-api-openapi.yml
  format: yaml
  label: edinetdb-jp Screener API
  slug: edinetdb-jp-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-screener-api-openapi.yml
- filename: edinetdb-jp-search-api-openapi.yml
  format: yaml
  label: edinetdb-jp Search API
  slug: edinetdb-jp-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-search-api-openapi.yml
- filename: edinetdb-jp-shareholders-api-openapi.yml
  format: yaml
  label: edinetdb-jp Shareholders API
  slug: edinetdb-jp-shareholders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-shareholders-api-openapi.yml
- filename: edinetdb-jp-subsidiaries-api-openapi.yml
  format: yaml
  label: edinetdb-jp Subsidiaries API
  slug: edinetdb-jp-subsidiaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-subsidiaries-api-openapi.yml
- filename: edinetdb-jp-system-api-openapi.yml
  format: yaml
  label: edinetdb-jp System API
  slug: edinetdb-jp-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-system-api-openapi.yml
- filename: edinetdb-jp-watchlist-api-openapi.yml
  format: yaml
  label: edinetdb-jp Watchlist API
  slug: edinetdb-jp-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edinetdb-jp/openapi/edinetdb-jp-watchlist-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Edinetdb Jp Authentication
name_suffix: Authentication
oauth_flows: []
overview: edinetdb-jp declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: edinetdb-jp
provider_slug: edinetdb-jp
scheme_count: 2
schemes:
- description: API key authentication.
  in: header
  name: X-API-Key
  type: apiKey
- description: Bearer token authentication (alternative to API key).
  scheme: bearer
  type: http
slug: edinetdb-jp-authentication
source_filename: edinetdb-jp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/edinetdb-jp-openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key authentication.\n  - type: http\n    scheme: bearer\n    description: Bearer token authentication (alternative to API key).\n"
source_yaml_url: https://artifacts.apis.io/edinetdb-jp/authentication/edinetdb-jp-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Data
- API
- Japan
- EDINET
---
