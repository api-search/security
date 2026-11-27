---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuasense-com-analysis-analysis-api-openapi.yml
  format: yaml
  label: NuaSense Analysis Analysis API
  slug: nuasense-com-analysis-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-analysis-analysis-api-openapi.yml
- filename: nuasense-com-analysis-demand-api-openapi.yml
  format: yaml
  label: NuaSense Analysis Demand API
  slug: nuasense-com-analysis-demand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-analysis-demand-api-openapi.yml
- filename: nuasense-com-analysis-news-api-openapi.yml
  format: yaml
  label: NuaSense Analysis News API
  slug: nuasense-com-analysis-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-analysis-news-api-openapi.yml
- filename: nuasense-com-analysis-prices-api-openapi.yml
  format: yaml
  label: NuaSense Analysis Prices API
  slug: nuasense-com-analysis-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-analysis-prices-api-openapi.yml
- filename: nuasense-com-catalog-api-openapi.yml
  format: yaml
  label: NuaSense Catalog API
  slug: nuasense-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-catalog-api-openapi.yml
- filename: nuasense-com-farm-api-openapi.yml
  format: yaml
  label: NuaSense Farm API
  slug: nuasense-com-farm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-farm-api-openapi.yml
- filename: nuasense-com-market-api-openapi.yml
  format: yaml
  label: NuaSense Market API
  slug: nuasense-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuasense-com/openapi/nuasense-com-market-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NuaSense Authentication
name_suffix: Authentication
oauth_flows: []
overview: NuaSense secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NuaSense
provider_slug: nuasense-com
scheme_count: 1
schemes:
- description: API key from https://platform.nuasense.com/manage/keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nuasense-com-openapi.json
  type: http
slug: nuasense-com-authentication
source_filename: nuasense-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nuasense-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key from https://platform.nuasense.com/manage/keys\n  sources:\n  - openapi/nuasense-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nuasense-com/authentication/nuasense-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Agriculture
- IoT
- Sensors
- Data Analytics
- Kenya
- Company
---
