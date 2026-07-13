---
api_key_in: []
api_specs:
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Access Token API
  slug: vagaro-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Appointments API
  slug: vagaro-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Customers API
  slug: vagaro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employees API
  slug: vagaro-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employee Management API
  slug: vagaro-employee-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Locations API
  slug: vagaro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vagaro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vagaro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vagaro
provider_slug: vagaro
scheme_count: 1
schemes:
- bearerFormat: token issued by /merchants/generate-access-token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vagaro-openapi.yml
  type: http
slug: vagaro-authentication
source_filename: vagaro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vagaro-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token issued by /merchants/generate-access-token\n  sources:\n  - openapi/vagaro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/authentication/vagaro-authentication.yml
summary_line: http · 1 scheme
tags:
- Salon
- Spa
- Fitness
- Wellness
- Scheduling
- Booking
- Vertical SaaS
---
