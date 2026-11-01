---
anonymous_access: false
api_key_in: []
api_specs:
- filename: startup-jobs-companies-api-openapi.yml
  format: yaml
  label: startup-jobs Companies API
  slug: startup-jobs-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-companies-api-openapi.yml
- filename: startup-jobs-jobs-api-openapi.yml
  format: yaml
  label: startup-jobs Jobs API
  slug: startup-jobs-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-jobs-api-openapi.yml
- filename: startup-jobs-locations-api-openapi.yml
  format: yaml
  label: startup-jobs Locations API
  slug: startup-jobs-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-locations-api-openapi.yml
- filename: startup-jobs-openapi-json-api-openapi.yml
  format: yaml
  label: startup-jobs Openapi.json API
  slug: startup-jobs-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-openapi-json-api-openapi.yml
- filename: startup-jobs-roles-api-openapi.yml
  format: yaml
  label: startup-jobs Roles API
  slug: startup-jobs-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-roles-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Startup Jobs Authentication
name_suffix: Authentication
oauth_flows: []
overview: startup-jobs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: startup-jobs
provider_slug: startup-jobs
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API key passed as Bearer token in Authorization header or as `api_key` query parameter.
  scheme: bearer
  type: http
slug: startup-jobs-authentication
source_filename: startup-jobs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://api.startup.jobs/v1/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key passed as Bearer token in Authorization header or as `api_key` query parameter.\n"
source_yaml_url: https://artifacts.apis.io/startup-jobs/authentication/startup-jobs-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
