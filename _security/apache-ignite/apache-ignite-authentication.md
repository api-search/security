---
api_key_in: []
api_specs:
- filename: apache-ignite-rest-api.yaml
  format: yaml
  label: Apache Ignite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Ignite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Ignite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Ignite
provider_slug: apache-ignite
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-ignite-rest-api.yaml
  type: http
slug: apache-ignite-authentication
source_filename: apache-ignite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-ignite-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-ignite-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/authentication/apache-ignite-authentication.yml
summary_line: http · 1 scheme
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
---
