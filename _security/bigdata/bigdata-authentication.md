---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bigdata-analyst-estimates-api-openapi.yml
  format: yaml
  label: RavenPack Analyst Estimates API
  slug: bigdata-analyst-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-analyst-estimates-api-openapi.yml
- filename: bigdata-company-events-api-openapi.yml
  format: yaml
  label: RavenPack Company & Events API
  slug: bigdata-company-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-company-events-api-openapi.yml
- filename: bigdata-financials-ratios-api-openapi.yml
  format: yaml
  label: RavenPack Financials & Ratios API
  slug: bigdata-financials-ratios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-financials-ratios-api-openapi.yml
- filename: bigdata-fixed-income-api-openapi.yml
  format: yaml
  label: RavenPack Fixed Income API
  slug: bigdata-fixed-income-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-fixed-income-api-openapi.yml
- filename: bigdata-fund-holdings-api-openapi.yml
  format: yaml
  label: RavenPack Fund Holdings API
  slug: bigdata-fund-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-fund-holdings-api-openapi.yml
- filename: bigdata-market-data-api-openapi.yml
  format: yaml
  label: RavenPack Market Data API
  slug: bigdata-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-market-data-api-openapi.yml
- filename: bigdata-private-markets-api-openapi.yml
  format: yaml
  label: RavenPack Private Markets API
  slug: bigdata-private-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bigdata/openapi/bigdata-private-markets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bigdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: RavenPack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RavenPack
provider_slug: bigdata
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/bigdata-structured_data.json
  type: apiKey
slug: bigdata-authentication
source_filename: bigdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/bigdata-structured_data.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/bigdata-structured_data.json\n"
source_yaml_url: https://artifacts.apis.io/bigdata/authentication/bigdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Finance
- Artificial Intelligence
- Data Analytics
- Market Insights
---
