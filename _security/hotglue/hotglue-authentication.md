---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: hotglue-jobs-api-openapi.yml
  format: yaml
  label: Hotglue Jobs API
  slug: hotglue-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-jobs-api-openapi.yml
- filename: hotglue-availableconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Available Connectors API
  slug: hotglue-availableconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availableconnectors-api-openapi.yml
- filename: hotglue-availablesources-api-openapi.yml
  format: yaml
  label: Hotglue Available Sources API
  slug: hotglue-availablesources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availablesources-api-openapi.yml
- filename: hotglue-availabletargets-api-openapi.yml
  format: yaml
  label: Hotglue Available Targets API
  slug: hotglue-availabletargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-availabletargets-api-openapi.yml
- filename: hotglue-connectors-api-openapi.yml
  format: yaml
  label: Hotglue Connectors API
  slug: hotglue-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-connectors-api-openapi.yml
- filename: hotglue-flows-api-openapi.yml
  format: yaml
  label: Hotglue Flows API
  slug: hotglue-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-flows-api-openapi.yml
- filename: hotglue-jupyter-api-openapi.yml
  format: yaml
  label: Hotglue Jupyter API
  slug: hotglue-jupyter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-jupyter-api-openapi.yml
- filename: hotglue-linkedconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Linked Connectors API
  slug: hotglue-linkedconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedconnectors-api-openapi.yml
- filename: hotglue-linkedsources-api-openapi.yml
  format: yaml
  label: Hotglue Linked Sources API
  slug: hotglue-linkedsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedsources-api-openapi.yml
- filename: hotglue-linkedtargets-api-openapi.yml
  format: yaml
  label: Hotglue Linked Targets API
  slug: hotglue-linkedtargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-linkedtargets-api-openapi.yml
- filename: hotglue-mcptoken-api-openapi.yml
  format: yaml
  label: Hotglue MCP Token API
  slug: hotglue-mcptoken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-mcptoken-api-openapi.yml
- filename: hotglue-supportedconnectors-api-openapi.yml
  format: yaml
  label: Hotglue Supported Connectors API
  slug: hotglue-supportedconnectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedconnectors-api-openapi.yml
- filename: hotglue-supportedsources-api-openapi.yml
  format: yaml
  label: Hotglue Supported Sources API
  slug: hotglue-supportedsources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedsources-api-openapi.yml
- filename: hotglue-supportedtargets-api-openapi.yml
  format: yaml
  label: Hotglue Supported Targets API
  slug: hotglue-supportedtargets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-supportedtargets-api-openapi.yml
- filename: hotglue-tenant-api-openapi.yml
  format: yaml
  label: Hotglue Tenant API
  slug: hotglue-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-tenant-api-openapi.yml
- filename: hotglue-tenants-api-openapi.yml
  format: yaml
  label: Hotglue Tenants API
  slug: hotglue-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-tenants-api-openapi.yml
- filename: hotglue-magic-link-api-openapi.yml
  format: yaml
  label: Hotglue Magic Link API
  slug: hotglue-magic-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hotglue/openapi/hotglue-magic-link-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hotglue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hotglue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hotglue
provider_slug: hotglue
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/hotglue-openapi.yml
  type: apiKey
slug: hotglue-authentication
source_filename: hotglue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hotglue-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/hotglue-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/hotglue/authentication/hotglue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Connectors
- Embedded Integrations
- ETL
- Integration Platform
- iPaaS
---
