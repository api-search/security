---
api_key_in: []
api_specs:
- filename: apache-kylin-rest-api.yaml
  format: yaml
  label: Apache Kylin REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Kylin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Kylin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Kylin
provider_slug: apache-kylin
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-kylin-rest-api.yaml
  type: http
slug: apache-kylin-authentication
source_filename: apache-kylin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-kylin-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-kylin-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/authentication/apache-kylin-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
---
