---
anonymous_access: false
api_key_in: []
api_specs:
- filename: astronomer-mux-create-upload-api-openapi.yml
  format: yaml
  label: Astronomer Mux Create Upload API
  slug: astronomer-mux-create-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astronomer/openapi/astronomer-mux-create-upload-api-openapi.yml
- filename: astronomer-mux-get-playback-id-api-openapi.yml
  format: yaml
  label: Astronomer Mux Get Playback Id API
  slug: astronomer-mux-get-playback-id-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astronomer/openapi/astronomer-mux-get-playback-id-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Astronomer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astronomer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Astronomer
provider_slug: astronomer
scheme_count: 1
schemes:
- name: JWT
  scheme: bearer
  sources:
  - openapi/astronomer-astro-openapi-original.yml
  type: http
slug: astronomer-authentication
source_filename: astronomer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/astronomer-astro-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/astronomer-astro-openapi-original.yml\n"
source_yaml_url: https://artifacts.apis.io/astronomer/authentication/astronomer-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Orchestration
- Apache Airflow
- Data Pipeline
- Data Engineering
- Workflow Automation
- MLOps
- Managed Platform
---
