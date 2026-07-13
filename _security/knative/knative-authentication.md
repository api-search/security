---
api_key_in: []
api_specs:
- filename: knative-serving-api-openapi.yml
  format: yaml
  label: Knative Serving API
  slug: knative-serving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-serving-api-openapi.yml
- filename: knative-eventing-api-openapi.yml
  format: yaml
  label: Knative Eventing API
  slug: knative-eventing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventing-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knative Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knative secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knative
provider_slug: knative
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Kubernetes service account token or user bearer token. RBAC policies control access to Knative Eventing resources.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/knative-eventing-api-openapi.yml
  - openapi/knative-serving-api-openapi.yml
  type: http
slug: knative-authentication
source_filename: knative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knative-eventing-api-openapi.yml, openapi/knative-serving-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account token or user bearer token. RBAC policies control\n    access to Knative Eventing resources.\n  sources:\n  - openapi/knative-eventing-api-openapi.yml\n  - openapi/knative-serving-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/authentication/knative-authentication.yml
summary_line: http · 1 scheme
tags:
- Auto-Scaling
- Cloud Native
- Event-Driven
- Graduated
- Kubernetes
- Serverless
---
