---
api_key_in:
- query
api_specs:
- filename: nacos-auth-api-openapi.yml
  format: yaml
  label: Nacos Auth API
  slug: nacos-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-auth-api-openapi.yml
- filename: nacos-configuration-api-openapi.yml
  format: yaml
  label: Nacos Configuration API
  slug: nacos-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-configuration-api-openapi.yml
- filename: nacos-namespace-api-openapi.yml
  format: yaml
  label: Nacos Namespace API
  slug: nacos-namespace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-namespace-api-openapi.yml
- filename: nacos-operator-api-openapi.yml
  format: yaml
  label: Nacos Operator API
  slug: nacos-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-operator-api-openapi.yml
- filename: nacos-service-discovery-api-openapi.yml
  format: yaml
  label: Nacos Service Discovery API
  slug: nacos-service-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-service-discovery-api-openapi.yml
- filename: nacos-service-management-api-openapi.yml
  format: yaml
  label: Nacos Service Management API
  slug: nacos-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-service-management-api-openapi.yml
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
