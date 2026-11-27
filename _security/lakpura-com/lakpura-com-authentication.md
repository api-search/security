---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lakpura-com-authentication-api-openapi.yml
  format: yaml
  label: Lakpura Authentication API
  slug: lakpura-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-authentication-api-openapi.yml
- filename: lakpura-com-customers-api-openapi.yml
  format: yaml
  label: Lakpura Customers API
  slug: lakpura-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-customers-api-openapi.yml
- filename: lakpura-com-jobs-api-openapi.yml
  format: yaml
  label: Lakpura Jobs API
  slug: lakpura-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-jobs-api-openapi.yml
- filename: lakpura-com-notifications-api-openapi.yml
  format: yaml
  label: Lakpura Notifications API
  slug: lakpura-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-notifications-api-openapi.yml
- filename: lakpura-com-users-api-openapi.yml
  format: yaml
  label: Lakpura Users API
  slug: lakpura-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lakpura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lakpura secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lakpura
provider_slug: lakpura-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lakpura-com-openapi.yaml
  type: http
slug: lakpura-com-authentication
source_filename: lakpura-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/lakpura-com-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lakpura-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/lakpura-com/authentication/lakpura-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- E-Commerce
- IT Services
- Sri Lanka
- Marketplace
---
