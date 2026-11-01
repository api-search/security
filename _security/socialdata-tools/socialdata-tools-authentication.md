---
anonymous_access: false
api_key_in: []
api_specs:
- filename: socialdata-tools-data-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Data API
  slug: socialdata-tools-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-data-api-api-openapi.yml
- filename: socialdata-tools-monitoring-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Monitoring API
  slug: socialdata-tools-monitoring-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-monitoring-api-api-openapi.yml
- filename: socialdata-tools-social-actions-api-api-openapi.yml
  format: yaml
  label: socialdata-tools Social Actions API
  slug: socialdata-tools-social-actions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-social-actions-api-api-openapi.yml
- filename: socialdata-tools-socialdata-account-management-api-openapi.yml
  format: yaml
  label: socialdata-tools SocialData Account Management API
  slug: socialdata-tools-socialdata-account-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialdata-tools/openapi/socialdata-tools-socialdata-account-management-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Socialdata Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: socialdata-tools declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: socialdata-tools
provider_slug: socialdata-tools
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: API key provided as Bearer token in Authorization header
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: socialdata-tools-authentication
source_filename: socialdata-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.socialdata.tools/getting-started/authentication/\nschemes:\n  - type: http\n    scheme: bearer\n    description: API key provided as Bearer token in Authorization header\n    bearerFormat: JWT\n    name: Authorization\n    in: header\n"
source_yaml_url: https://artifacts.apis.io/socialdata-tools/authentication/socialdata-tools-authentication.yml
summary_line: 1 scheme
tags:
- API
- Data
- Social Media
- X
- Twitter
---
