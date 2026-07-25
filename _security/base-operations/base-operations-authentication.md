---
api_key_in:
- header
api_specs:
- filename: base-operations-analytics-api-openapi.yml
  format: yaml
  label: Base Operations Analytics API
  slug: base-operations-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-analytics-api-openapi.yml
- filename: base-operations-base-score-api-openapi.yml
  format: yaml
  label: Base Operations Base Score API
  slug: base-operations-base-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-base-score-api-openapi.yml
- filename: base-operations-change-detection-api-openapi.yml
  format: yaml
  label: Base Operations Change Detection API
  slug: base-operations-change-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-change-detection-api-openapi.yml
- filename: base-operations-key-takeaways-api-openapi.yml
  format: yaml
  label: Base Operations Key Takeaways API
  slug: base-operations-key-takeaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-key-takeaways-api-openapi.yml
- filename: base-operations-public-charts-api-openapi.yml
  format: yaml
  label: Base Operations Public Charts API
  slug: base-operations-public-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-public-charts-api-openapi.yml
- filename: base-operations-radius-charts-api-openapi.yml
  format: yaml
  label: Base Operations Radius Charts API
  slug: base-operations-radius-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-radius-charts-api-openapi.yml
- filename: base-operations-saved-location-charts-api-openapi.yml
  format: yaml
  label: Base Operations Saved Location Charts API
  slug: base-operations-saved-location-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-location-charts-api-openapi.yml
- filename: base-operations-saved-location-radius-charts-api-openapi.yml
  format: yaml
  label: Base Operations Saved Location Radius Charts API
  slug: base-operations-saved-location-radius-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-location-radius-charts-api-openapi.yml
- filename: base-operations-saved-locations-api-openapi.yml
  format: yaml
  label: Base Operations Saved Locations API
  slug: base-operations-saved-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-locations-api-openapi.yml
- filename: base-operations-source-categories-api-openapi.yml
  format: yaml
  label: Base Operations Source Categories API
  slug: base-operations-source-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-source-categories-api-openapi.yml
- filename: base-operations-threat-categories-api-openapi.yml
  format: yaml
  label: Base Operations Threat Categories API
  slug: base-operations-threat-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-threat-categories-api-openapi.yml
- filename: base-operations-threats-api-openapi.yml
  format: yaml
  label: Base Operations Threats API
  slug: base-operations-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-threats-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Base Operations Authentication
name_suffix: Authentication
oauth_flows: []
overview: Base Operations secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Base Operations
provider_slug: base-operations
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: X-API-KEY
  sources:
  - openapi/base-operations-openapi-original.json
  type: apiKey
slug: base-operations-authentication
source_filename: base-operations-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/base-operations-openapi-original.json\ndocs: https://www.baseoperations.com/product/api\ndetail: Include your unique API key in the X-API-KEY header with each request.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/base-operations-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/authentication/base-operations-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Threat Intelligence
- Security
- Risk Management
- Physical Security
- Crime Data
- Geospatial
- Public Safety
- Risk Scoring
---
