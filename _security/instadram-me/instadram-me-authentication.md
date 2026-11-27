---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instadram-me-activity-api-openapi.yml
  format: yaml
  label: Instadram Activity API
  slug: instadram-me-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-activity-api-openapi.yml
- filename: instadram-me-bottles-api-openapi.yml
  format: yaml
  label: Instadram Bottles API
  slug: instadram-me-bottles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-bottles-api-openapi.yml
- filename: instadram-me-cocktails-api-openapi.yml
  format: yaml
  label: Instadram Cocktails API
  slug: instadram-me-cocktails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-cocktails-api-openapi.yml
- filename: instadram-me-collections-api-openapi.yml
  format: yaml
  label: Instadram Collections API
  slug: instadram-me-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-collections-api-openapi.yml
- filename: instadram-me-expressions-api-openapi.yml
  format: yaml
  label: Instadram Expressions API
  slug: instadram-me-expressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-expressions-api-openapi.yml
- filename: instadram-me-search-api-openapi.yml
  format: yaml
  label: Instadram Search API
  slug: instadram-me-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-search-api-openapi.yml
- filename: instadram-me-users-api-openapi.yml
  format: yaml
  label: Instadram Users API
  slug: instadram-me-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instadram-me/openapi/instadram-me-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Instadram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instadram secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instadram
provider_slug: instadram-me
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Firebase Auth JWT token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instadram-me-openapi.yml
  type: http
slug: instadram-me-authentication
source_filename: instadram-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/instadram-me-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Firebase Auth JWT token\n  sources:\n  - openapi/instadram-me-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/instadram-me/authentication/instadram-me-authentication.yml
summary_line: http · 1 scheme
tags:
- Whiskey inventory
- Bottle scanner
- Tasting journal
---
