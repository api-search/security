---
api_key_in: []
api_specs:
- filename: scalable-services-configmaps-api-openapi.yml
  format: yaml
  label: Scalable Services ConfigMaps API
  slug: scalable-services-configmaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-configmaps-api-openapi.yml
- filename: scalable-services-namespaces-api-openapi.yml
  format: yaml
  label: Scalable Services Namespaces API
  slug: scalable-services-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-namespaces-api-openapi.yml
- filename: scalable-services-nodes-api-openapi.yml
  format: yaml
  label: Scalable Services Nodes API
  slug: scalable-services-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-nodes-api-openapi.yml
- filename: scalable-services-persistentvolumes-api-openapi.yml
  format: yaml
  label: Scalable Services PersistentVolumes API
  slug: scalable-services-persistentvolumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-persistentvolumes-api-openapi.yml
- filename: scalable-services-pods-api-openapi.yml
  format: yaml
  label: Scalable Services Pods API
  slug: scalable-services-pods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-pods-api-openapi.yml
- filename: scalable-services-secrets-api-openapi.yml
  format: yaml
  label: Scalable Services Secrets API
  slug: scalable-services-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-secrets-api-openapi.yml
- filename: scalable-services-services-api-openapi.yml
  format: yaml
  label: Scalable Services Services API
  slug: scalable-services-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/openapi/scalable-services-services-api-openapi.yml
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
