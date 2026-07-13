---
api_key_in: []
api_specs:
- filename: apache-james-webadmin-rest-api.yaml
  format: yaml
  label: Apache James WebAdmin REST API
  slug: webadmin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-webadmin-rest-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache James Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache James secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache James
provider_slug: apache-james
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apache-james-webadmin-rest-api.yaml
  type: http
slug: apache-james-authentication
source_filename: apache-james-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-james-webadmin-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/apache-james-webadmin-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/authentication/apache-james-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
---
