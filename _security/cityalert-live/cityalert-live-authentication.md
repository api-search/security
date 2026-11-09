---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cityalert-live-agents-api-openapi.yml
  format: yaml
  label: CityAlert.live Agents API
  slug: cityalert-live-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-agents-api-openapi.yml
- filename: cityalert-live-community-api-openapi.yml
  format: yaml
  label: CityAlert.live Community API
  slug: cityalert-live-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-community-api-openapi.yml
- filename: cityalert-live-feeds-api-openapi.yml
  format: yaml
  label: CityAlert.live Feeds API
  slug: cityalert-live-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-feeds-api-openapi.yml
- filename: cityalert-live-history-api-openapi.yml
  format: yaml
  label: CityAlert.live History API
  slug: cityalert-live-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-history-api-openapi.yml
- filename: cityalert-live-incidents-api-openapi.yml
  format: yaml
  label: CityAlert.live Incidents API
  slug: cityalert-live-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-incidents-api-openapi.yml
- filename: cityalert-live-meta-api-openapi.yml
  format: yaml
  label: CityAlert.live Meta API
  slug: cityalert-live-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-meta-api-openapi.yml
- filename: cityalert-live-news-api-openapi.yml
  format: yaml
  label: CityAlert.live News API
  slug: cityalert-live-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-news-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cityalert Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: CityAlert.live secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CityAlert.live
provider_slug: cityalert-live
scheme_count: 1
schemes:
- description: Paid API key (ca_…) — see /developers for plan tiers
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/cityalert-live-openapi.json
  type: apiKey
slug: cityalert-live-authentication
source_filename: cityalert-live-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cityalert-live-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Paid API key (ca_…) — see /developers for plan tiers\n  sources:\n  - openapi/cityalert-live-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cityalert-live/authentication/cityalert-live-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Safety
- Mapping
- Real-Time
- Open Data
- Community
---
