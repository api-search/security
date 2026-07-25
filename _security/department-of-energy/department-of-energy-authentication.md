---
api_key_in:
- query
api_specs:
- filename: department-of-energy-aeo-api-openapi.yml
  format: yaml
  label: Department of Energy Aeo API
  slug: department-of-energy-aeo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-aeo-api-openapi.yml
- filename: department-of-energy-co2-emissions-api-openapi.yml
  format: yaml
  label: Department of Energy Co2 Emissions API
  slug: department-of-energy-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-co2-emissions-api-openapi.yml
- filename: department-of-energy-coal-api-openapi.yml
  format: yaml
  label: Department of Energy Coal API
  slug: department-of-energy-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-coal-api-openapi.yml
- filename: department-of-energy-eia-open-data-api-v2-api-openapi.yml
  format: yaml
  label: Department of Energy EIA Open Data API V2 API
  slug: department-of-energy-eia-open-data-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-eia-open-data-api-v2-api-openapi.yml
- filename: department-of-energy-electricity-api-openapi.yml
  format: yaml
  label: Department of Energy Electricity API
  slug: department-of-energy-electricity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-electricity-api-openapi.yml
- filename: department-of-energy-international-api-openapi.yml
  format: yaml
  label: Department of Energy International API
  slug: department-of-energy-international-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-international-api-openapi.yml
- filename: department-of-energy-natural-gas-api-openapi.yml
  format: yaml
  label: Department of Energy Natural Gas API
  slug: department-of-energy-natural-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-natural-gas-api-openapi.yml
- filename: department-of-energy-nuclear-outages-api-openapi.yml
  format: yaml
  label: Department of Energy Nuclear Outages API
  slug: department-of-energy-nuclear-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-nuclear-outages-api-openapi.yml
- filename: department-of-energy-petroleum-api-openapi.yml
  format: yaml
  label: Department of Energy Petroleum API
  slug: department-of-energy-petroleum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-petroleum-api-openapi.yml
- filename: department-of-energy-seds-api-openapi.yml
  format: yaml
  label: Department of Energy Seds API
  slug: department-of-energy-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-seds-api-openapi.yml
- filename: department-of-energy-seriesid-api-openapi.yml
  format: yaml
  label: Department of Energy Seriesid API
  slug: department-of-energy-seriesid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-seriesid-api-openapi.yml
- filename: department-of-energy-steo-api-openapi.yml
  format: yaml
  label: Department of Energy Steo API
  slug: department-of-energy-steo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-steo-api-openapi.yml
- filename: department-of-energy-total-energy-api-openapi.yml
  format: yaml
  label: Department of Energy Total Energy API
  slug: department-of-energy-total-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/openapi/department-of-energy-total-energy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Energy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Energy
provider_slug: department-of-energy
scheme_count: 1
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/department-of-energy-openapi.yml
  type: apiKey
slug: department-of-energy-authentication
source_filename: department-of-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/department-of-energy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/department-of-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-energy/refs/heads/main/authentication/department-of-energy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Buildings
- Electricity
- Energy
- Federal Government
- Open Data
- Renewables
- Research
- Solar
- Statistics
---
