---
api_key_in:
- cookie
api_specs:
- filename: 9.0.5
  format: yaml
  label: WebSphere Application Server Admin API
  slug: websphere-admin-rest-api
  spec_type: OpenAPI
  url: https://www.ibm.com/docs/en/was/9.0.5?topic=api-openapi-specification
- filename: websphere-liberty-admin-rest-api.yml
  format: yaml
  label: WebSphere Liberty Admin REST API
  slug: websphere-liberty-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-admin-rest-api.yml
- filename: websphere-liberty-rest-connector-api.yml
  format: yaml
  label: WebSphere Liberty REST Connector API
  slug: websphere-liberty-rest-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-rest-connector-api.yml
- filename: websphere-mq-rest-api.yml
  format: yaml
  label: WebSphere MQ REST API
  slug: websphere-mq-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-mq-rest-api.yml
- filename: websphere-liberty-collective-controller-rest-api.yml
  format: yaml
  label: WebSphere Liberty Collective Controller REST API
  slug: websphere-liberty-collective-controller-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-liberty-collective-controller-rest-api.yml
- filename: websphere-automation-rest-api.yml
  format: yaml
  label: WebSphere Automation REST API
  slug: websphere-automation-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/websphere-automation-rest-api.yml
- filename: open-liberty-apis.yml
  format: yaml
  label: Open Liberty APIs
  slug: open-liberty-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/openapi/open-liberty-apis.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Websphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: IBM WebSphere secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IBM WebSphere
provider_slug: websphere
scheme_count: 3
schemes:
- description: HTTP Basic authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/open-liberty-apis.yml
  - openapi/websphere-admin-rest-api.yml
  - openapi/websphere-liberty-admin-rest-api.yml
  - openapi/websphere-liberty-collective-controller-rest-api.yml
  - openapi/websphere-liberty-rest-connector-api.yml
  - openapi/websphere-mq-rest-api.yml
  type: http
- bearerFormat: JWT
  description: MicroProfile JWT authentication
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/open-liberty-apis.yml
  - openapi/websphere-automation-rest-api.yml
  type: http
- description: LTPA token-based authentication
  in: cookie
  name: ltpaToken
  parameter: LtpaToken2
  sources:
  - openapi/websphere-admin-rest-api.yml
  - openapi/websphere-liberty-admin-rest-api.yml
  - openapi/websphere-mq-rest-api.yml
  type: apiKey
slug: websphere-authentication
source_filename: websphere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-liberty-apis.yml, openapi/websphere-admin-rest-api.yml, openapi/websphere-automation-rest-api.yml,\n  openapi/websphere-liberty-admin-rest-api.yml, openapi/websphere-liberty-collective-controller-rest-api.yml,\n  openapi/websphere-liberty-rest-connector-api.yml, openapi/websphere-mq-rest-api.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication\n  sources:\n  - openapi/open-liberty-apis.yml\n  - openapi/websphere-admin-rest-api.yml\n  - openapi/websphere-liberty-admin-rest-api.yml\n  - openapi/websphere-liberty-collective-controller-rest-api.yml\n  - openapi/websphere-liberty-rest-connector-api.yml\n  - openapi/websphere-mq-rest-api.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: MicroProfile JWT authentication\n  sources:\n  - openapi/open-liberty-apis.yml\n\
  \  - openapi/websphere-automation-rest-api.yml\n- name: ltpaToken\n  type: apiKey\n  in: cookie\n  parameter: LtpaToken2\n  description: LTPA token-based authentication\n  sources:\n  - openapi/websphere-admin-rest-api.yml\n  - openapi/websphere-liberty-admin-rest-api.yml\n  - openapi/websphere-mq-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/authentication/websphere-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
---
