---
api_key_in:
- header
api_specs:
- filename: land-insight-additional-opportunities-api-openapi.yml
  format: yaml
  label: Land Insight Additional Opportunities API
  slug: land-insight-additional-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-additional-opportunities-api-openapi.yml
- filename: land-insight-development-constraints-api-openapi.yml
  format: yaml
  label: Land Insight Development Constraints API
  slug: land-insight-development-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-development-constraints-api-openapi.yml
- filename: land-insight-development-opportunities-api-openapi.yml
  format: yaml
  label: Land Insight Development Opportunities API
  slug: land-insight-development-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-development-opportunities-api-openapi.yml
- filename: land-insight-getting-started-api-openapi.yml
  format: yaml
  label: Land Insight Getting Started API
  slug: land-insight-getting-started-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-getting-started-api-openapi.yml
- filename: land-insight-land-availability-assessment-api-openapi.yml
  format: yaml
  label: Land Insight Land Availability Assessment API
  slug: land-insight-land-availability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-land-availability-assessment-api-openapi.yml
- filename: land-insight-local-policy-api-openapi.yml
  format: yaml
  label: Land Insight Local Policy API
  slug: land-insight-local-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-local-policy-api-openapi.yml
- filename: land-insight-ownership-api-openapi.yml
  format: yaml
  label: Land Insight Ownership API
  slug: land-insight-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-ownership-api-openapi.yml
- filename: land-insight-parcels-api-openapi.yml
  format: yaml
  label: Land Insight Parcels API
  slug: land-insight-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-parcels-api-openapi.yml
- filename: land-insight-planning-applications-api-openapi.yml
  format: yaml
  label: Land Insight Planning Applications API
  slug: land-insight-planning-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-planning-applications-api-openapi.yml
- filename: land-insight-power-api-openapi.yml
  format: yaml
  label: Land Insight Power API
  slug: land-insight-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-power-api-openapi.yml
- filename: land-insight-renewable-energy-planning-db-api-openapi.yml
  format: yaml
  label: Land Insight Renewable Energy Planning DB API
  slug: land-insight-renewable-energy-planning-db-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-renewable-energy-planning-db-api-openapi.yml
- filename: land-insight-strategic-industrial-location-api-openapi.yml
  format: yaml
  label: Land Insight Strategic Industrial Location API
  slug: land-insight-strategic-industrial-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/openapi/land-insight-strategic-industrial-location-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Land Insight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Land Insight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Land Insight
provider_slug: land-insight
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/land-insight-api-openapi.yml
  type: apiKey
slug: land-insight-authentication
source_filename: land-insight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/land-insight-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/land-insight-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/land-insight/refs/heads/main/authentication/land-insight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Real Estate
- Property
- Land
- Planning
- Geospatial
- Data
- United Kingdom
- PropTech
- Construction
---
