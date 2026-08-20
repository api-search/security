---
api_key_in:
- query
api_specs:
- filename: energy-information-administration-co2-emissions-api-openapi.yml
  format: yaml
  label: Energy Information Administration CO2 Emissions API
  slug: energy-information-administration-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-co2-emissions-api-openapi.yml
- filename: energy-information-administration-coal-api-openapi.yml
  format: yaml
  label: Energy Information Administration Coal API
  slug: energy-information-administration-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-coal-api-openapi.yml
- filename: energy-information-administration-discovery-api-openapi.yml
  format: yaml
  label: Energy Information Administration Discovery API
  slug: energy-information-administration-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-discovery-api-openapi.yml
- filename: energy-information-administration-electricity-api-openapi.yml
  format: yaml
  label: Energy Information Administration Electricity API
  slug: energy-information-administration-electricity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-electricity-api-openapi.yml
- filename: energy-information-administration-international-api-openapi.yml
  format: yaml
  label: Energy Information Administration International API
  slug: energy-information-administration-international-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-international-api-openapi.yml
- filename: energy-information-administration-natural-gas-api-openapi.yml
  format: yaml
  label: Energy Information Administration Natural Gas API
  slug: energy-information-administration-natural-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-natural-gas-api-openapi.yml
- filename: energy-information-administration-nuclear-api-openapi.yml
  format: yaml
  label: Energy Information Administration Nuclear API
  slug: energy-information-administration-nuclear-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-nuclear-api-openapi.yml
- filename: energy-information-administration-petroleum-api-openapi.yml
  format: yaml
  label: Energy Information Administration Petroleum API
  slug: energy-information-administration-petroleum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-petroleum-api-openapi.yml
- filename: energy-information-administration-seds-api-openapi.yml
  format: yaml
  label: Energy Information Administration SEDS API
  slug: energy-information-administration-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-seds-api-openapi.yml
- filename: energy-information-administration-total-energy-api-openapi.yml
  format: yaml
  label: Energy Information Administration Total Energy API
  slug: energy-information-administration-total-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/openapi/energy-information-administration-total-energy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Energy Information Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Energy Information Administration secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Energy Information Administration
provider_slug: energy-information-administration
scheme_count: 1
schemes:
- description: Free API key obtained at https://www.eia.gov/opendata/register.php. Must be supplied on every request as the api_key URL parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/energy-information-administration-open-data-api-openapi.yml
  type: apiKey
slug: energy-information-administration-authentication
source_filename: energy-information-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/energy-information-administration-open-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Free API key obtained at https://www.eia.gov/opendata/register.php. Must be supplied\n    on every request as the api_key URL parameter.\n  sources:\n  - openapi/energy-information-administration-open-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-information-administration/refs/heads/main/authentication/energy-information-administration-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Federal-Government
- Open Data
---
