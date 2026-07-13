---
api_key_in: []
api_specs:
- filename: apache-ranger-rest-api.yaml
  format: yaml
  label: Apache Ranger REST API
  slug: apache-ranger-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Ranger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Ranger secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Ranger
provider_slug: apache-ranger
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-ranger-rest-api.yaml
  type: http
slug: apache-ranger-authentication
source_filename: apache-ranger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-ranger-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-ranger-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/authentication/apache-ranger-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
---
