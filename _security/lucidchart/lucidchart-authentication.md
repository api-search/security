---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lucidchart-groups-api-openapi.yml
  format: yaml
  label: Lucidchart Groups API
  slug: lucidchart-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucidchart/openapi/lucidchart-groups-api-openapi.yml
- filename: lucidchart-schemas-api-openapi.yml
  format: yaml
  label: Lucidchart Schemas API
  slug: lucidchart-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucidchart/openapi/lucidchart-schemas-api-openapi.yml
- filename: lucidchart-service-provider-config-api-openapi.yml
  format: yaml
  label: Lucidchart Service Provider Config API
  slug: lucidchart-service-provider-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucidchart/openapi/lucidchart-service-provider-config-api-openapi.yml
- filename: lucidchart-users-api-openapi.yml
  format: yaml
  label: Lucidchart Users API
  slug: lucidchart-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucidchart/openapi/lucidchart-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lucidchart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucidchart secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lucidchart
provider_slug: lucidchart
scheme_count: 1
schemes:
- bearerFormat: OAuth 2.0 access token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lucidchart-openapi.yml
  type: http
slug: lucidchart-authentication
source_filename: lucidchart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lucidchart-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.0 access token\n  sources:\n  - openapi/lucidchart-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lucidchart/authentication/lucidchart-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Diagramming
- Visualization
- Visual Workspace
- Software-as-a-Service
---
