---
api_key_in: []
api_specs:
- filename: apache-ranger-audit-api-openapi.yml
  format: yaml
  label: Apache Ranger Audit API
  slug: apache-ranger-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-audit-api-openapi.yml
- filename: apache-ranger-groups-api-openapi.yml
  format: yaml
  label: Apache Ranger Groups API
  slug: apache-ranger-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-groups-api-openapi.yml
- filename: apache-ranger-policies-api-openapi.yml
  format: yaml
  label: Apache Ranger Policies API
  slug: apache-ranger-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-policies-api-openapi.yml
- filename: apache-ranger-services-api-openapi.yml
  format: yaml
  label: Apache Ranger Services API
  slug: apache-ranger-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-services-api-openapi.yml
- filename: apache-ranger-users-api-openapi.yml
  format: yaml
  label: Apache Ranger Users API
  slug: apache-ranger-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/openapi/apache-ranger-users-api-openapi.yml
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
- Open-Source
---
