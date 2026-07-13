---
api_key_in: []
api_specs:
- filename: apache-knox-admin-api.yaml
  format: yaml
  label: Apache Knox Admin REST API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/openapi/apache-knox-admin-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Knox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Knox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Knox
provider_slug: apache-knox
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-knox-admin-api.yaml
  type: http
slug: apache-knox-authentication
source_filename: apache-knox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-knox-admin-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-knox-admin-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/authentication/apache-knox-authentication.yml
summary_line: http · 1 scheme
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
---
