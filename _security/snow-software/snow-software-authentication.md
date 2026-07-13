---
api_key_in: []
api_specs:
- filename: snow-software-licenses-openapi.yml
  format: yaml
  label: Snow Atlas SAM Licenses API
  slug: snow-atlas-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-licenses-openapi.yml
- filename: snow-software-saas-applications-openapi.yml
  format: yaml
  label: Snow Atlas SaaS Applications API
  slug: snow-atlas-saas-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-saas-applications-openapi.yml
- filename: snow-software-saas-subscriptions-openapi.yml
  format: yaml
  label: Snow Atlas SaaS Subscriptions API
  slug: snow-atlas-saas-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-saas-subscriptions-openapi.yml
- filename: snow-software-computers-openapi.json
  format: json
  label: Snow Atlas SAM Computers API
  slug: snow-atlas-computers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-computers-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snow Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snow Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snow Software
provider_slug: snow-software
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/snow-software-licenses-openapi.yml
  - openapi/snow-software-saas-applications-openapi.yml
  - openapi/snow-software-saas-subscriptions-openapi.yml
  type: http
slug: snow-software-authentication
source_filename: snow-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snow-software-licenses-openapi.yml, openapi/snow-software-saas-applications-openapi.yml,\n  openapi/snow-software-saas-subscriptions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/snow-software-licenses-openapi.yml\n  - openapi/snow-software-saas-applications-openapi.yml\n  - openapi/snow-software-saas-subscriptions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/authentication/snow-software-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud License Management
- FinOps
- IT Asset Management
- SaaS Management
- Software Asset Management
---
