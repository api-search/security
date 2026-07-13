---
api_key_in: []
api_specs:
- filename: spring-boot-actuator-openapi.yml
  format: yaml
  label: Spring Boot Actuator API
  slug: spring-boot-actuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-boot-actuator-openapi.yml
- filename: spring-initializr-api-openapi.yml
  format: yaml
  label: Spring Initializr API
  slug: spring-initializr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-initializr-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spring Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spring Framework secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spring Framework
provider_slug: spring
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/spring-boot-actuator-openapi.yml
  type: http
slug: spring-authentication
source_filename: spring-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spring-boot-actuator-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/spring-boot-actuator-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/authentication/spring-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Cloud Native
- Enterprise
- Framework
- Java
- Microservices
- Open Source
- REST
- Spring Boot
---
