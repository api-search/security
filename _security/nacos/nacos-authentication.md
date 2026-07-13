---
api_key_in:
- query
api_specs:
- filename: nacos-open-api.yml
  format: yaml
  label: Nacos
  slug: nacos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-open-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nacos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nacos secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nacos
provider_slug: nacos
scheme_count: 1
schemes:
- description: Access token obtained from login endpoint
  in: query
  name: AccessToken
  parameter: accessToken
  sources:
  - openapi/nacos-open-api.yml
  type: apiKey
slug: nacos-authentication
source_filename: nacos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nacos-open-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: Access token obtained from login endpoint\n  sources:\n  - openapi/nacos-open-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/authentication/nacos-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Alibaba
- Cloud Native
- Configuration Management
- DNS
- Java
- Microservices
- Service Discovery
- Service Management
---
