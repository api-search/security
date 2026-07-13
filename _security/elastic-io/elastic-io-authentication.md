---
api_key_in: []
api_specs:
- filename: elastic-io-platform-api-openapi.yml
  format: yaml
  label: Elastic.io
  slug: elastic-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/openapi/elastic-io-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Elastic Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elastic.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Elastic.io
provider_slug: elastic-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication. Obtain a token through the elastic.io platform login or API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/elastic-io-platform-api-openapi.yml
  type: http
slug: elastic-io-authentication
source_filename: elastic-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elastic-io-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication. Obtain a token through the elastic.io platform login\n    or API key.\n  sources:\n  - openapi/elastic-io-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/authentication/elastic-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Integrations
- iPaaS
- SaaS Integration
---
