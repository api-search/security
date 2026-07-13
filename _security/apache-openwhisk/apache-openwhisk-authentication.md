---
api_key_in: []
api_specs:
- filename: apache-openwhisk-rest-api.yaml
  format: yaml
  label: Apache OpenWhisk REST API
  slug: apache-openwhisk-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/openapi/apache-openwhisk-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Openwhisk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache OpenWhisk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
scheme_count: 1
schemes:
- description: HTTP Basic authentication using OpenWhisk credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-openwhisk-rest-api.yaml
  type: http
slug: apache-openwhisk-authentication
source_filename: apache-openwhisk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-openwhisk-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using OpenWhisk credentials\n  sources:\n  - openapi/apache-openwhisk-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/authentication/apache-openwhisk-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
---
