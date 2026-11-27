---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fulcradynamics-com-annotations-api-openapi.yml
  format: yaml
  label: Fulcra Annotations API
  slug: fulcradynamics-com-annotations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-annotations-api-openapi.yml
- filename: fulcradynamics-com-calendars-api-openapi.yml
  format: yaml
  label: Fulcra Calendars API
  slug: fulcradynamics-com-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-calendars-api-openapi.yml
- filename: fulcradynamics-com-data-api-openapi.yml
  format: yaml
  label: Fulcra Data API
  slug: fulcradynamics-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-data-api-openapi.yml
- filename: fulcradynamics-com-data-types-api-openapi.yml
  format: yaml
  label: Fulcra Data Types API
  slug: fulcradynamics-com-data-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-data-types-api-openapi.yml
- filename: fulcradynamics-com-file-uploads-api-openapi.yml
  format: yaml
  label: Fulcra file uploads API
  slug: fulcradynamics-com-file-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-file-uploads-api-openapi.yml
- filename: fulcradynamics-com-files-api-openapi.yml
  format: yaml
  label: Fulcra Files API
  slug: fulcradynamics-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-files-api-openapi.yml
- filename: fulcradynamics-com-ingest-api-openapi.yml
  format: yaml
  label: Fulcra Ingest API
  slug: fulcradynamics-com-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-ingest-api-openapi.yml
- filename: fulcradynamics-com-location-api-openapi.yml
  format: yaml
  label: Fulcra Location API
  slug: fulcradynamics-com-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-location-api-openapi.yml
- filename: fulcradynamics-com-sleep-api-openapi.yml
  format: yaml
  label: Fulcra Sleep API
  slug: fulcradynamics-com-sleep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-sleep-api-openapi.yml
- filename: fulcradynamics-com-tags-api-openapi.yml
  format: yaml
  label: Fulcra Tags API
  slug: fulcradynamics-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-tags-api-openapi.yml
- filename: fulcradynamics-com-user-api-openapi.yml
  format: yaml
  label: Fulcra User API
  slug: fulcradynamics-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fulcradynamics-com/openapi/fulcradynamics-com-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fulcra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fulcra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fulcra
provider_slug: fulcradynamics-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fulcradynamics-com-openapi.json
  type: http
slug: fulcradynamics-com-authentication
source_filename: fulcradynamics-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/fulcradynamics-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fulcradynamics-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fulcradynamics-com/authentication/fulcradynamics-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Context
- Backend
- Agents
- Platform
---
