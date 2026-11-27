---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aleva-se-aviation-api-openapi.yml
  format: yaml
  label: Aleva Aviation API
  slug: aleva-se-aviation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-aviation-api-openapi.yml
- filename: aleva-se-courts-api-openapi.yml
  format: yaml
  label: Aleva Courts API
  slug: aleva-se-courts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-courts-api-openapi.yml
- filename: aleva-se-domains-api-openapi.yml
  format: yaml
  label: Aleva Domains API
  slug: aleva-se-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-domains-api-openapi.yml
- filename: aleva-se-economy-api-openapi.yml
  format: yaml
  label: Aleva Economy API
  slug: aleva-se-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-economy-api-openapi.yml
- filename: aleva-se-energy-api-openapi.yml
  format: yaml
  label: Aleva Energy API
  slug: aleva-se-energy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-energy-api-openapi.yml
- filename: aleva-se-foods-api-openapi.yml
  format: yaml
  label: Aleva Foods API
  slug: aleva-se-foods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-foods-api-openapi.yml
- filename: aleva-se-jobs-api-openapi.yml
  format: yaml
  label: Aleva Jobs API
  slug: aleva-se-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-jobs-api-openapi.yml
- filename: aleva-se-medicines-api-openapi.yml
  format: yaml
  label: Aleva Medicines API
  slug: aleva-se-medicines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-medicines-api-openapi.yml
- filename: aleva-se-municipalities-api-openapi.yml
  format: yaml
  label: Aleva Municipalities API
  slug: aleva-se-municipalities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-municipalities-api-openapi.yml
- filename: aleva-se-rates-api-openapi.yml
  format: yaml
  label: Aleva Rates API
  slug: aleva-se-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-rates-api-openapi.yml
- filename: aleva-se-riksdag-api-openapi.yml
  format: yaml
  label: Aleva Riksdag API
  slug: aleva-se-riksdag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-riksdag-api-openapi.yml
- filename: aleva-se-stats-api-openapi.yml
  format: yaml
  label: Aleva Stats API
  slug: aleva-se-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-stats-api-openapi.yml
- filename: aleva-se-sweden-api-openapi.yml
  format: yaml
  label: Aleva Sweden API
  slug: aleva-se-sweden-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-sweden-api-openapi.yml
- filename: aleva-se-tourism-api-openapi.yml
  format: yaml
  label: Aleva Tourism API
  slug: aleva-se-tourism-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-tourism-api-openapi.yml
- filename: aleva-se-trains-api-openapi.yml
  format: yaml
  label: Aleva Trains API
  slug: aleva-se-trains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-trains-api-openapi.yml
- filename: aleva-se-weather-api-openapi.yml
  format: yaml
  label: Aleva Weather API
  slug: aleva-se-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-weather-api-openapi.yml
- filename: aleva-se-web-api-openapi.yml
  format: yaml
  label: Aleva Web API
  slug: aleva-se-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aleva-se/openapi/aleva-se-web-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aleva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aleva declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aleva
provider_slug: aleva-se
scheme_count: 2
schemes:
- description: Optional API key for higher limits.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Optional bearer token for higher limits.
  scheme: bearer
  type: http
slug: aleva-se-authentication
source_filename: aleva-se-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://aleva.se/docs#auth\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: Optional API key for higher limits.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Optional bearer token for higher limits.\n"
source_yaml_url: https://artifacts.apis.io/aleva-se/authentication/aleva-se-authentication.yml
summary_line: 2 schemes
tags:
- Swedish
- Data Infrastructure
- Artificial Intelligence
- Open Data
- Government Data
---
