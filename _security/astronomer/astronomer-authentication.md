---
api_key_in: []
api_specs:
- filename: astronomer-astro-openapi-original.yml
  format: yaml
  label: Astro Platform API
  slug: astro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-astro-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/authentication/astronomer-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Orchestration
- Apache Airflow
- Data Pipelines
- Data Engineering
- Workflow Automation
- MLOps
- Managed Platform
---
