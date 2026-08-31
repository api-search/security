---
api_key_in: []
api_specs:
- filename: apache-kylin-authentication-api-openapi.yml
  format: yaml
  label: Apache Kylin Authentication API
  slug: apache-kylin-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-authentication-api-openapi.yml
- filename: apache-kylin-jobs-api-openapi.yml
  format: yaml
  label: Apache Kylin Jobs API
  slug: apache-kylin-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-jobs-api-openapi.yml
- filename: apache-kylin-models-api-openapi.yml
  format: yaml
  label: Apache Kylin Models API
  slug: apache-kylin-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-models-api-openapi.yml
- filename: apache-kylin-projects-api-openapi.yml
  format: yaml
  label: Apache Kylin Projects API
  slug: apache-kylin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-projects-api-openapi.yml
- filename: apache-kylin-query-api-openapi.yml
  format: yaml
  label: Apache Kylin Query API
  slug: apache-kylin-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-query-api-openapi.yml
- filename: apache-kylin-tables-api-openapi.yml
  format: yaml
  label: Apache Kylin Tables API
  slug: apache-kylin-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/openapi/apache-kylin-tables-api-openapi.yml
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
- Open-Source
- SQL
---
