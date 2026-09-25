---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: vital-io-aggregate-api-openapi.yml
  format: yaml
  label: Vital Aggregate API
  slug: vital-io-aggregate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-aggregate-api-openapi.yml
- filename: vital-io-compendium-api-openapi.yml
  format: yaml
  label: Vital Compendium API
  slug: vital-io-compendium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-compendium-api-openapi.yml
- filename: vital-io-insurance-api-openapi.yml
  format: yaml
  label: Vital Insurance API
  slug: vital-io-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-insurance-api-openapi.yml
- filename: vital-io-introspect-api-openapi.yml
  format: yaml
  label: Vital Introspect API
  slug: vital-io-introspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-introspect-api-openapi.yml
- filename: vital-io-lab-account-api-openapi.yml
  format: yaml
  label: Vital Lab Account API
  slug: vital-io-lab-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-account-api-openapi.yml
- filename: vital-io-lab-report-api-openapi.yml
  format: yaml
  label: Vital Lab Report API
  slug: vital-io-lab-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-report-api-openapi.yml
- filename: vital-io-lab-tests-api-openapi.yml
  format: yaml
  label: Vital Lab Tests API
  slug: vital-io-lab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-tests-api-openapi.yml
- filename: vital-io-link-api-openapi.yml
  format: yaml
  label: Vital Link API
  slug: vital-io-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-link-api-openapi.yml
- filename: vital-io-order-api-openapi.yml
  format: yaml
  label: Vital Order API
  slug: vital-io-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-order-api-openapi.yml
- filename: vital-io-order-transaction-api-openapi.yml
  format: yaml
  label: Vital Order Transaction API
  slug: vital-io-order-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-order-transaction-api-openapi.yml
- filename: vital-io-orders-api-openapi.yml
  format: yaml
  label: Vital Orders API
  slug: vital-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-orders-api-openapi.yml
- filename: vital-io-payor-api-openapi.yml
  format: yaml
  label: Vital Payor API
  slug: vital-io-payor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-payor-api-openapi.yml
- filename: vital-io-providers-api-openapi.yml
  format: yaml
  label: Vital Providers API
  slug: vital-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-providers-api-openapi.yml
- filename: vital-io-summary-api-openapi.yml
  format: yaml
  label: Vital Summary API
  slug: vital-io-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-summary-api-openapi.yml
- filename: vital-io-team-api-openapi.yml
  format: yaml
  label: Vital Team API
  slug: vital-io-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-team-api-openapi.yml
- filename: vital-io-user-api-openapi.yml
  format: yaml
  label: Vital User API
  slug: vital-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-user-api-openapi.yml
- filename: vital-io-aggregation-api-openapi.yml
  format: yaml
  label: Vital Aggregation API
  slug: vital-io-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-aggregation-api-openapi.yml
- filename: vital-io-lab-testing-api-openapi.yml
  format: yaml
  label: Vital Lab Testing API
  slug: vital-io-lab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-testing-api-openapi.yml
- filename: vital-io-time-series-api-openapi.yml
  format: yaml
  label: Vital Time Series API
  slug: vital-io-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-time-series-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- Health Tech
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
- Webhook
- Phlebotomy
- Lab Orders
---
