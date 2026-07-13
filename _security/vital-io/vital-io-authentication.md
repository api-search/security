---
api_key_in:
- header
api_specs:
- filename: vital-users-api-openapi.yml
  format: yaml
  label: Vital Users API
  slug: vital-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-users-api-openapi.yml
- filename: vital-link-api-openapi.yml
  format: yaml
  label: Vital Link API
  slug: vital-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-link-api-openapi.yml
- filename: vital-wearables-api-openapi.yml
  format: yaml
  label: Vital Wearables Data API
  slug: vital-wearables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-wearables-api-openapi.yml
- filename: vital-lab-testing-api-openapi.yml
  format: yaml
  label: Vital Lab Testing API
  slug: vital-lab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-testing-api-openapi.yml
- filename: vital-lab-report-parser-api-openapi.yml
  format: yaml
  label: Vital Lab Report Parser API
  slug: vital-lab-report-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-report-parser-api-openapi.yml
- filename: vital-sense-api-openapi.yml
  format: yaml
  label: Vital Sense API
  slug: vital-sense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-sense-api-openapi.yml
- filename: vital-team-api-openapi.yml
  format: yaml
  label: Vital Team API
  slug: vital-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-team-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vital Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vital secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vital
provider_slug: vital-io
scheme_count: 1
schemes:
- description: Vital Team API Key
  in: header
  name: apiKeyAuth
  parameter: x-vital-api-key
  sources:
  - openapi/vital-lab-report-parser-api-openapi.yml
  - openapi/vital-lab-testing-api-openapi.yml
  - openapi/vital-link-api-openapi.yml
  - openapi/vital-openapi-original.json
  - openapi/vital-openapi-original.yml
  - openapi/vital-sense-api-openapi.yml
  - openapi/vital-team-api-openapi.yml
  - openapi/vital-users-api-openapi.yml
  - openapi/vital-wearables-api-openapi.yml
  type: apiKey
slug: vital-io-authentication
source_filename: vital-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vital-lab-report-parser-api-openapi.yml, openapi/vital-lab-testing-api-openapi.yml,\n  openapi/vital-link-api-openapi.yml, openapi/vital-openapi-original.json, openapi/vital-openapi-original.yml,\n  openapi/vital-sense-api-openapi.yml, openapi/vital-team-api-openapi.yml, openapi/vital-users-api-openapi.yml,\n  openapi/vital-wearables-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-vital-api-key\n  description: Vital Team API Key\n  sources:\n  - openapi/vital-lab-report-parser-api-openapi.yml\n  - openapi/vital-lab-testing-api-openapi.yml\n  - openapi/vital-link-api-openapi.yml\n  - openapi/vital-openapi-original.json\n  - openapi/vital-openapi-original.yml\n  - openapi/vital-sense-api-openapi.yml\n  - openapi/vital-team-api-openapi.yml\n  - openapi/vital-users-api-openapi.yml\n  - openapi/vital-wearables-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/authentication/vital-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Health Data
- Wearables
- Lab Testing
- Digital Health
- Healthtech
- Healthcare
- HIPAA
- HealthKit
- Health Connect
- EHR
- EMR
- Biomarkers
- Diagnostics
- Continuous Glucose Monitoring
- Sleep
- Activity
- Heart Rate
- Webhooks
- Phlebotomy
- Lab Orders
---
