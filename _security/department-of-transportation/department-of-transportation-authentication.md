---
api_key_in:
- query
api_specs:
- filename: department-of-transportation-airport-status-api-openapi.yml
  format: yaml
  label: Department of Transportation Airport Status API
  slug: department-of-transportation-airport-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-airport-status-api-openapi.yml
- filename: department-of-transportation-authority-api-openapi.yml
  format: yaml
  label: Department of Transportation Authority API
  slug: department-of-transportation-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-authority-api-openapi.yml
- filename: department-of-transportation-carriers-api-openapi.yml
  format: yaml
  label: Department of Transportation Carriers API
  slug: department-of-transportation-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-carriers-api-openapi.yml
- filename: department-of-transportation-complaints-api-openapi.yml
  format: yaml
  label: Department of Transportation Complaints API
  slug: department-of-transportation-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-complaints-api-openapi.yml
- filename: department-of-transportation-crashes-api-openapi.yml
  format: yaml
  label: Department of Transportation Crashes API
  slug: department-of-transportation-crashes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-crashes-api-openapi.yml
- filename: department-of-transportation-inspections-api-openapi.yml
  format: yaml
  label: Department of Transportation Inspections API
  slug: department-of-transportation-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-inspections-api-openapi.yml
- filename: department-of-transportation-makes-api-openapi.yml
  format: yaml
  label: Department of Transportation Makes API
  slug: department-of-transportation-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-makes-api-openapi.yml
- filename: department-of-transportation-manufacturers-api-openapi.yml
  format: yaml
  label: Department of Transportation Manufacturers API
  slug: department-of-transportation-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-manufacturers-api-openapi.yml
- filename: department-of-transportation-models-api-openapi.yml
  format: yaml
  label: Department of Transportation Models API
  slug: department-of-transportation-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-models-api-openapi.yml
- filename: department-of-transportation-ratings-api-openapi.yml
  format: yaml
  label: Department of Transportation Ratings API
  slug: department-of-transportation-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-ratings-api-openapi.yml
- filename: department-of-transportation-recalls-api-openapi.yml
  format: yaml
  label: Department of Transportation Recalls API
  slug: department-of-transportation-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-recalls-api-openapi.yml
- filename: department-of-transportation-vehicle-variables-api-openapi.yml
  format: yaml
  label: Department of Transportation Vehicle Variables API
  slug: department-of-transportation-vehicle-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vehicle-variables-api-openapi.yml
- filename: department-of-transportation-vin-decode-api-openapi.yml
  format: yaml
  label: Department of Transportation VIN Decode API
  slug: department-of-transportation-vin-decode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-vin-decode-api-openapi.yml
- filename: department-of-transportation-wmi-api-openapi.yml
  format: yaml
  label: Department of Transportation WMI API
  slug: department-of-transportation-wmi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/openapi/department-of-transportation-wmi-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of Transportation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Transportation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Transportation
provider_slug: department-of-transportation
scheme_count: 1
schemes:
- in: query
  name: WebKey
  parameter: webKey
  sources:
  - openapi/fmcsa-qcmobile-api-openapi.yml
  type: apiKey
slug: department-of-transportation-authentication
source_filename: department-of-transportation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fmcsa-qcmobile-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: WebKey\n  type: apiKey\n  in: query\n  parameter: webKey\n  sources:\n  - openapi/fmcsa-qcmobile-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/authentication/department-of-transportation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
---
