---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emnify-applicationtokens-api-openapi.yml
  format: yaml
  label: emnify Application Tokens API
  slug: emnify-applicationtokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-applicationtokens-api-openapi.yml
- filename: emnify-authentication-api-openapi.yml
  format: yaml
  label: emnify Authentication API
  slug: emnify-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-authentication-api-openapi.yml
- filename: emnify-cloudconnect-api-openapi.yml
  format: yaml
  label: emnify Cloud Connect API
  slug: emnify-cloudconnect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-cloudconnect-api-openapi.yml
- filename: emnify-endpoint-api-openapi.yml
  format: yaml
  label: emnify Endpoint API
  slug: emnify-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-endpoint-api-openapi.yml
- filename: emnify-events-api-openapi.yml
  format: yaml
  label: emnify Events API
  slug: emnify-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-events-api-openapi.yml
- filename: emnify-flowlogs-api-openapi.yml
  format: yaml
  label: emnify Flow Logs API
  slug: emnify-flowlogs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-flowlogs-api-openapi.yml
- filename: emnify-integrations-api-openapi.yml
  format: yaml
  label: emnify Integrations API
  slug: emnify-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-integrations-api-openapi.yml
- filename: emnify-ipaddressspaces-api-openapi.yml
  format: yaml
  label: emnify Ip Address Spaces API
  slug: emnify-ipaddressspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-ipaddressspaces-api-openapi.yml
- filename: emnify-lookups-api-openapi.yml
  format: yaml
  label: emnify Lookups API
  slug: emnify-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-lookups-api-openapi.yml
- filename: emnify-operator-api-openapi.yml
  format: yaml
  label: emnify Operator API
  slug: emnify-operator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-operator-api-openapi.yml
- filename: emnify-organization-api-openapi.yml
  format: yaml
  label: emnify Organization API
  slug: emnify-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-organization-api-openapi.yml
- filename: emnify-passwordmanagementandactivation-api-openapi.yml
  format: yaml
  label: emnify Password Management And Activation API
  slug: emnify-passwordmanagementandactivation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-passwordmanagementandactivation-api-openapi.yml
- filename: emnify-permissionandrolemanagement-api-openapi.yml
  format: yaml
  label: emnify Permission And Role Management API
  slug: emnify-permissionandrolemanagement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-permissionandrolemanagement-api-openapi.yml
- filename: emnify-servicelookupsandconfiguration-api-openapi.yml
  format: yaml
  label: emnify Service Lookups And Configuration API
  slug: emnify-servicelookupsandconfiguration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-servicelookupsandconfiguration-api-openapi.yml
- filename: emnify-serviceprofiles-api-openapi.yml
  format: yaml
  label: emnify Service Profiles API
  slug: emnify-serviceprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-serviceprofiles-api-openapi.yml
- filename: emnify-sim-api-openapi.yml
  format: yaml
  label: emnify Sim API
  slug: emnify-sim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-sim-api-openapi.yml
- filename: emnify-tagmanagement-api-openapi.yml
  format: yaml
  label: emnify Tag Management API
  slug: emnify-tagmanagement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-tagmanagement-api-openapi.yml
- filename: emnify-tariffplans-api-openapi.yml
  format: yaml
  label: emnify Tariff Plans API
  slug: emnify-tariffplans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-tariffplans-api-openapi.yml
- filename: emnify-tariffprofiles-api-openapi.yml
  format: yaml
  label: emnify Tariff Profiles API
  slug: emnify-tariffprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-tariffprofiles-api-openapi.yml
- filename: emnify-workspaces-api-openapi.yml
  format: yaml
  label: emnify Workspaces API
  slug: emnify-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-workspaces-api-openapi.yml
- filename: emnify-user-management-api-openapi.yml
  format: yaml
  label: emnify User Management API
  slug: emnify-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emnify/openapi/emnify-user-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Emnify Authentication
name_suffix: Authentication
oauth_flows: []
overview: emnify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: emnify
provider_slug: emnify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Retrieve a JWT via POST /api/v1/authenticate using an application_token or user credentials, then send it as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/emnify-api-openapi.yml
  type: http
slug: emnify-authentication
source_filename: emnify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emnify-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Retrieve a JWT via POST /api/v1/authenticate using an application_token or user\n    credentials, then send it as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/emnify-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/emnify/authentication/emnify-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Cellular Connectivity
- IoT SIM
- eSIM
- Consumer eSIM
- SGP.32
- M2M
- NTN-IoT
- Satellite
- SuperNetwork
- Machine-to-Machine
---
