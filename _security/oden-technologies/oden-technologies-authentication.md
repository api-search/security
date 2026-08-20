---
api_key_in:
- header
api_specs:
- filename: oden-technologies-dashboards-api-openapi.yml
  format: yaml
  label: Oden Technologies Dashboards API
  slug: oden-technologies-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-dashboards-api-openapi.yml
- filename: oden-technologies-intervals-api-openapi.yml
  format: yaml
  label: Oden Technologies Intervals API
  slug: oden-technologies-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-intervals-api-openapi.yml
- filename: oden-technologies-machine-groups-api-openapi.yml
  format: yaml
  label: Oden Technologies Machine Groups API
  slug: oden-technologies-machine-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-machine-groups-api-openapi.yml
- filename: oden-technologies-maintenance-work-orders-api-openapi.yml
  format: yaml
  label: Oden Technologies Maintenance Work Orders API
  slug: oden-technologies-maintenance-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-maintenance-work-orders-api-openapi.yml
- filename: oden-technologies-metric-groups-api-openapi.yml
  format: yaml
  label: Oden Technologies Metric Groups API
  slug: oden-technologies-metric-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-metric-groups-api-openapi.yml
- filename: oden-technologies-oql-api-openapi.yml
  format: yaml
  label: Oden Technologies OQL API
  slug: oden-technologies-oql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-oql-api-openapi.yml
- filename: oden-technologies-product-attributes-api-openapi.yml
  format: yaml
  label: Oden Technologies Product Attributes API
  slug: oden-technologies-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-product-attributes-api-openapi.yml
- filename: oden-technologies-product-mappings-api-openapi.yml
  format: yaml
  label: Oden Technologies Product Mappings API
  slug: oden-technologies-product-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-product-mappings-api-openapi.yml
- filename: oden-technologies-products-api-openapi.yml
  format: yaml
  label: Oden Technologies Products API
  slug: oden-technologies-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-products-api-openapi.yml
- filename: oden-technologies-quality-test-api-openapi.yml
  format: yaml
  label: Oden Technologies Quality Test API
  slug: oden-technologies-quality-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-quality-test-api-openapi.yml
- filename: oden-technologies-scrap-yield-data-api-openapi.yml
  format: yaml
  label: Oden Technologies Scrap/Yield Data API
  slug: oden-technologies-scrap-yield-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-scrap-yield-data-api-openapi.yml
- filename: oden-technologies-targets-api-openapi.yml
  format: yaml
  label: Oden Technologies Targets API
  slug: oden-technologies-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-targets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oden Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oden Technologies secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oden Technologies
provider_slug: oden-technologies
scheme_count: 1
schemes:
- description: Prefix the value with \"Token\" to indicate the custom authorization type
  in: header
  name: APIKeyAuth
  parameter: Authorization
  sources:
  - openapi/oden-technologies-openapi-original.yml
  type: apiKey
slug: oden-technologies-authentication
source_filename: oden-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oden-technologies-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Prefix the value with \\\"Token\\\" to indicate the custom authorization type\n  sources:\n  - openapi/oden-technologies-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/authentication/oden-technologies-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Manufacturing
- Industrial IoT
- Analytics
- Artificial Intelligence
- Factory
- Manufacturing Analytics
---
