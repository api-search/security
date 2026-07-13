---
api_key_in: []
api_specs:
- filename: spring-cloud-config-server-api.yml
  format: yaml
  label: Spring Cloud Config Server API
  slug: spring-cloud-config-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-cloud-config/refs/heads/main/openapi/spring-cloud-config-server-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spring Cloud Config Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spring Cloud Config secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spring Cloud Config
provider_slug: spring-cloud-config
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/spring-cloud-config-server-api.yml
  type: http
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/spring-cloud-config-server-api.yml
  type: http
slug: spring-cloud-config-authentication
source_filename: spring-cloud-config-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spring-cloud-config-server-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/spring-cloud-config-server-api.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/spring-cloud-config-server-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-cloud-config/refs/heads/main/authentication/spring-cloud-config-authentication.yml
summary_line: http · 2 schemes
tags:
- Configuration Management
- Distributed Systems
- Externalized Configuration
- Git
- Java
- Microservices
- Spring
- Spring Cloud
---
