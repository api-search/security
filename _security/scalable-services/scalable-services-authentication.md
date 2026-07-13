---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: Kubernetes API
  slug: kubernetes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kubernetes/kubernetes/master/api/openapi-spec/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Services secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Services
provider_slug: scalable-services
scheme_count: 1
schemes:
- bearerFormat: ServiceAccountToken
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalable-services-openapi.yml
  type: http
slug: scalable-services-authentication
source_filename: scalable-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-services-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ServiceAccountToken\n  sources:\n  - openapi/scalable-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/authentication/scalable-services-authentication.yml
summary_line: http · 1 scheme
tags:
- API Gateway
- Cloud Native
- Containers
- Distributed Systems
- High Availability
- Kubernetes
- Load Balancing
- Microservices
- Scalable Architecture
- Serverless
- Service Mesh
---
