---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ubicquia-authcheck-api-openapi.yml
  format: yaml
  label: Ubicquia Auth Check API
  slug: ubicquia-authcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-authcheck-api-openapi.yml
- filename: ubicquia-customer-detail-api-openapi.yml
  format: yaml
  label: Ubicquia Customer Detail API
  slug: ubicquia-customer-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-customer-detail-api-openapi.yml
- filename: ubicquia-fulfillment-details-api-openapi.yml
  format: yaml
  label: Ubicquia Fulfillment Details API
  slug: ubicquia-fulfillment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-fulfillment-details-api-openapi.yml
- filename: ubicquia-iccid-master-api-openapi.yml
  format: yaml
  label: Ubicquia ICCID Master API
  slug: ubicquia-iccid-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-iccid-master-api-openapi.yml
- filename: ubicquia-sales-order-api-openapi.yml
  format: yaml
  label: Ubicquia Sales Order API
  slug: ubicquia-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-sales-order-api-openapi.yml
- filename: ubicquia-serial-number-api-openapi.yml
  format: yaml
  label: Ubicquia Serial Number API
  slug: ubicquia-serial-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-serial-number-api-openapi.yml
- filename: ubicquia-transformer-details-api-openapi.yml
  format: yaml
  label: Ubicquia Transformer Details API
  slug: ubicquia-transformer-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-transformer-details-api-openapi.yml
- filename: ubicquia-user-api-openapi.yml
  format: yaml
  label: Ubicquia User API
  slug: ubicquia-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/openapi/ubicquia-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ubicquia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubicquia secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ubicquia
provider_slug: ubicquia
scheme_count: 1
schemes:
- description: 'Use header x-api-key: ''key'' to send api key endpoints'
  in: header
  name: Api Key
  parameter: x-api-key
  sources:
  - openapi/ubicquia-config-api-openapi-original.json
  type: apiKey
slug: ubicquia-authentication
source_filename: ubicquia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nsource: openapi/ubicquia-config-api-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Api Key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Use header x-api-key: ''key'' to send api key endpoints'\n  sources:\n  - openapi/ubicquia-config-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubicquia/refs/heads/main/authentication/ubicquia-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Smart Cities
- IoT
- Energy
- Utilities
- Electric Grid
- Streetlights
- Public Safety
- Infrastructure
- Sensors
- Edge AI
- Transformer Monitoring
---
