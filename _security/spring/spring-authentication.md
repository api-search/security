---
api_key_in: []
api_specs:
- filename: spring-beans-api-openapi.yml
  format: yaml
  label: Spring Framework Beans API
  slug: spring-beans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-beans-api-openapi.yml
- filename: spring-environment-api-openapi.yml
  format: yaml
  label: Spring Framework Environment API
  slug: spring-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-environment-api-openapi.yml
- filename: spring-health-api-openapi.yml
  format: yaml
  label: Spring Framework Health API
  slug: spring-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-health-api-openapi.yml
- filename: spring-info-api-openapi.yml
  format: yaml
  label: Spring Framework Info API
  slug: spring-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-info-api-openapi.yml
- filename: spring-loggers-api-openapi.yml
  format: yaml
  label: Spring Framework Loggers API
  slug: spring-loggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-loggers-api-openapi.yml
- filename: spring-mappings-api-openapi.yml
  format: yaml
  label: Spring Framework Mappings API
  slug: spring-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-mappings-api-openapi.yml
- filename: spring-metadata-api-openapi.yml
  format: yaml
  label: Spring Framework Metadata API
  slug: spring-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-metadata-api-openapi.yml
- filename: spring-metrics-api-openapi.yml
  format: yaml
  label: Spring Framework Metrics API
  slug: spring-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-metrics-api-openapi.yml
- filename: spring-project-generation-api-openapi.yml
  format: yaml
  label: Spring Framework Project Generation API
  slug: spring-project-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-project-generation-api-openapi.yml
- filename: spring-threads-api-openapi.yml
  format: yaml
  label: Spring Framework Threads API
  slug: spring-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-threads-api-openapi.yml
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
- Artificial Intelligence
- Cloud-Native
- Enterprise
- Framework
- Java
- Microservices
- Open-Source
- REST
- Spring Boot
---
