---
api_key_in:
- header
- query
api_specs:
- filename: workwave-callback-api-openapi.yml
  format: yaml
  label: WorkWave Callback API
  slug: workwave-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-callback-api-openapi.yml
- filename: workwave-companies-api-openapi.yml
  format: yaml
  label: WorkWave Companies API
  slug: workwave-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-companies-api-openapi.yml
- filename: workwave-depots-api-openapi.yml
  format: yaml
  label: WorkWave Depots API
  slug: workwave-depots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-depots-api-openapi.yml
- filename: workwave-drivers-api-openapi.yml
  format: yaml
  label: WorkWave Drivers API
  slug: workwave-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-drivers-api-openapi.yml
- filename: workwave-gps-api-openapi.yml
  format: yaml
  label: WorkWave GPS API
  slug: workwave-gps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-gps-api-openapi.yml
- filename: workwave-orders-api-openapi.yml
  format: yaml
  label: WorkWave Orders API
  slug: workwave-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-orders-api-openapi.yml
- filename: workwave-regions-api-openapi.yml
  format: yaml
  label: WorkWave Regions API
  slug: workwave-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-regions-api-openapi.yml
- filename: workwave-routes-api-openapi.yml
  format: yaml
  label: WorkWave Routes API
  slug: workwave-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-routes-api-openapi.yml
- filename: workwave-territories-api-openapi.yml
  format: yaml
  label: WorkWave Territories API
  slug: workwave-territories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-territories-api-openapi.yml
- filename: workwave-validation-api-openapi.yml
  format: yaml
  label: WorkWave Validation API
  slug: workwave-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-validation-api-openapi.yml
- filename: workwave-vehicles-api-openapi.yml
  format: yaml
  label: WorkWave Vehicles API
  slug: workwave-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/openapi/workwave-vehicles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Workwave Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkWave secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WorkWave
provider_slug: workwave
scheme_count: 2
schemes:
- description: API key (UUID) supplied via the X-WorkWave-Key HTTP header.
  in: header
  name: ApiKeyHeader
  parameter: X-WorkWave-Key
  sources:
  - openapi/workwave-openapi.yml
  type: apiKey
- description: API key (UUID) supplied via the `key` query-string parameter. Takes precedence over the header if both are present.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/workwave-openapi.yml
  type: apiKey
slug: workwave-authentication
source_filename: workwave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workwave-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-WorkWave-Key\n  description: API key (UUID) supplied via the X-WorkWave-Key HTTP header.\n  sources:\n  - openapi/workwave-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key (UUID) supplied via the `key` query-string parameter. Takes precedence\n    over the header if both are present.\n  sources:\n  - openapi/workwave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workwave/refs/heads/main/authentication/workwave-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Field Service
- Route Optimization
- Last Mile Delivery
- Fleet
- GPS Tracking
- Logistics
---
