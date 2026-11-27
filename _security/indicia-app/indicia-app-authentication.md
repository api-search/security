---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: indicia-app-activity-api-openapi.yml
  format: yaml
  label: Indicia Activity API
  slug: indicia-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-activity-api-openapi.yml
- filename: indicia-app-infrastructure-api-openapi.yml
  format: yaml
  label: Indicia Infrastructure API
  slug: indicia-app-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-infrastructure-api-openapi.yml
- filename: indicia-app-intelligence-api-openapi.yml
  format: yaml
  label: Indicia Intelligence API
  slug: indicia-app-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-intelligence-api-openapi.yml
- filename: indicia-app-organizations-api-openapi.yml
  format: yaml
  label: Indicia Organizations API
  slug: indicia-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-organizations-api-openapi.yml
- filename: indicia-app-pricing-api-openapi.yml
  format: yaml
  label: Indicia Pricing API
  slug: indicia-app-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-pricing-api-openapi.yml
- filename: indicia-app-socials-api-openapi.yml
  format: yaml
  label: Indicia Socials API
  slug: indicia-app-socials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-socials-api-openapi.yml
- filename: indicia-app-tools-api-openapi.yml
  format: yaml
  label: Indicia Tools API
  slug: indicia-app-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-tools-api-openapi.yml
- filename: indicia-app-unified-api-openapi.yml
  format: yaml
  label: Indicia Unified API
  slug: indicia-app-unified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-unified-api-openapi.yml
- filename: indicia-app-users-api-openapi.yml
  format: yaml
  label: Indicia Users API
  slug: indicia-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicia-app/openapi/indicia-app-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Indicia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indicia secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Indicia
provider_slug: indicia-app
scheme_count: 2
schemes:
- description: API key for authenticating requests. Obtain a key from [Indicia Dashboard](https://indicia.app/dashboard/account)
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/indicia-app-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.1 access token issued by https://indicia.app/api/auth. Audience must be this API.
  name: OAuth2
  scheme: bearer
  sources:
  - openapi/indicia-app-openapi.json
  type: http
slug: indicia-app-authentication
source_filename: indicia-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/indicia-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for authenticating requests. Obtain a key from [Indicia Dashboard](https://indicia.app/dashboard/account)\n  sources:\n  - openapi/indicia-app-openapi.json\n- name: OAuth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.1 access token issued by https://indicia.app/api/auth. Audience must\n    be this API.\n  sources:\n  - openapi/indicia-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/indicia-app/authentication/indicia-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- OSINT
- Investigations
- Data Aggregation
- Cybersecurity
- Open Source
---
