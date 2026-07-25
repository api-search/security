---
api_key_in: []
api_specs:
- filename: climatiq-autopilot-api-openapi.yml
  format: yaml
  label: Climatiq Autopilot API
  slug: climatiq-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-autopilot-api-openapi.yml
- filename: climatiq-cbam-api-openapi.yml
  format: yaml
  label: Climatiq CBAM API
  slug: climatiq-cbam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-cbam-api-openapi.yml
- filename: climatiq-classifications-api-openapi.yml
  format: yaml
  label: Climatiq Classifications API
  slug: climatiq-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-classifications-api-openapi.yml
- filename: climatiq-computing-api-openapi.yml
  format: yaml
  label: Climatiq Computing API
  slug: climatiq-computing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-computing-api-openapi.yml
- filename: climatiq-energy-api-openapi.yml
  format: yaml
  label: Climatiq Energy API
  slug: climatiq-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-energy-api-openapi.yml
- filename: climatiq-estimate-api-openapi.yml
  format: yaml
  label: Climatiq Estimate API
  slug: climatiq-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-estimate-api-openapi.yml
- filename: climatiq-freight-api-openapi.yml
  format: yaml
  label: Climatiq Freight API
  slug: climatiq-freight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-freight-api-openapi.yml
- filename: climatiq-procurement-api-openapi.yml
  format: yaml
  label: Climatiq Procurement API
  slug: climatiq-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-procurement-api-openapi.yml
- filename: climatiq-reference-api-openapi.yml
  format: yaml
  label: Climatiq Reference API
  slug: climatiq-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-reference-api-openapi.yml
- filename: climatiq-search-api-openapi.yml
  format: yaml
  label: Climatiq Search API
  slug: climatiq-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-search-api-openapi.yml
- filename: climatiq-travel-api-openapi.yml
  format: yaml
  label: Climatiq Travel API
  slug: climatiq-travel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/openapi/climatiq-travel-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Climatiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Climatiq secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Climatiq
provider_slug: climatiq
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/climatiq-openapi.yml
  type: http
slug: climatiq-authentication
source_filename: climatiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/climatiq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/climatiq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climatiq/refs/heads/main/authentication/climatiq-authentication.yml
summary_line: http · 1 scheme
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Energy
- Environment
- GHG Protocol
- Sustainability
---
