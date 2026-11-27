---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mobilitydata-config-api-openapi.yml
  format: yaml
  label: MobilityData Config API
  slug: mobilitydata-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-config-api-openapi.yml
- filename: mobilitydata-early-access-api-openapi.yml
  format: yaml
  label: MobilityData Early Access API
  slug: mobilitydata-early-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-early-access-api-openapi.yml
- filename: mobilitydata-licenses-api-openapi.yml
  format: yaml
  label: MobilityData Licenses API
  slug: mobilitydata-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-licenses-api-openapi.yml
- filename: mobilitydata-notifications-api-openapi.yml
  format: yaml
  label: MobilityData Notifications API
  slug: mobilitydata-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-notifications-api-openapi.yml
- filename: mobilitydata-operations-api-openapi.yml
  format: yaml
  label: MobilityData Operations API
  slug: mobilitydata-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-operations-api-openapi.yml
- filename: mobilitydata-parquet-api-openapi.yml
  format: yaml
  label: MobilityData Parquet API
  slug: mobilitydata-parquet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-parquet-api-openapi.yml
- filename: mobilitydata-users-api-openapi.yml
  format: yaml
  label: MobilityData Users API
  slug: mobilitydata-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilitydata/openapi/mobilitydata-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MobilityData Authentication
name_suffix: Authentication
oauth_flows: []
overview: MobilityData secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MobilityData
provider_slug: mobilitydata
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/operationsapi.yaml
  type: apiKey
slug: mobilitydata-authentication
source_filename: mobilitydata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/operationsapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/operationsapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/mobilitydata/authentication/mobilitydata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Mobility
- Data Standards
- Open Source
- Non-Profit
- Transportation
---
