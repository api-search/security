---
api_key_in: []
api_specs:
- filename: apache-nutch-openapi.yaml
  format: yaml
  label: Apache Nutch REST API
  slug: apache-nutch-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Nutch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Nutch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Nutch
provider_slug: apache-nutch
scheme_count: 1
schemes:
- description: HTTP Basic Authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-nutch-openapi.yaml
  type: http
slug: apache-nutch-authentication
source_filename: apache-nutch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-nutch-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication.\n  sources:\n  - openapi/apache-nutch-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/authentication/apache-nutch-authentication.yml
summary_line: http · 1 scheme
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
---
