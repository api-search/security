---
anonymous_access: false
api_key_in: []
api_specs:
- filename: namesniper-pro-account-api-openapi.yml
  format: yaml
  label: NameSniper Account API
  slug: namesniper-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-account-api-openapi.yml
- filename: namesniper-pro-check-api-openapi.yml
  format: yaml
  label: NameSniper Check API
  slug: namesniper-pro-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-check-api-openapi.yml
- filename: namesniper-pro-generate-api-openapi.yml
  format: yaml
  label: NameSniper Generate API
  slug: namesniper-pro-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-generate-api-openapi.yml
- filename: namesniper-pro-monitoring-api-openapi.yml
  format: yaml
  label: NameSniper Monitoring API
  slug: namesniper-pro-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-monitoring-api-openapi.yml
- filename: namesniper-pro-trademark-api-openapi.yml
  format: yaml
  label: NameSniper Trademark API
  slug: namesniper-pro-trademark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-trademark-api-openapi.yml
- filename: namesniper-pro-webhooks-api-openapi.yml
  format: yaml
  label: NameSniper Webhooks API
  slug: namesniper-pro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NameSniper Authentication
name_suffix: Authentication
oauth_flows: []
overview: NameSniper secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NameSniper
provider_slug: namesniper-pro
scheme_count: 1
schemes:
- bearerFormat: ns_sk
  description: 'API key issued from the dashboard, sent as `Authorization: Bearer ns_sk_...`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/namesniper-pro-openapi.yaml
  type: http
slug: namesniper-pro-authentication
source_filename: namesniper-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/namesniper-pro-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ns_sk\n  description: 'API key issued from the dashboard, sent as `Authorization: Bearer ns_sk_...`.'\n  sources:\n  - openapi/namesniper-pro-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/namesniper-pro/authentication/namesniper-pro-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- UsernameChecker
- HandleMonitor
- Social Media
- Domain Search
---
