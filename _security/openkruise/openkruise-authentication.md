---
api_key_in: []
api_specs:
- filename: openkruise-openapi.yml
  format: yaml
  label: OpenKruise Workload API
  slug: openkruise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openkruise/refs/heads/main/openapi/openkruise-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openkruise Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenKruise secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenKruise
provider_slug: openkruise
scheme_count: 1
schemes:
- description: Kubernetes service account or user bearer token presented to the API server.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/openkruise-openapi.yml
  type: http
slug: openkruise-authentication
source_filename: openkruise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openkruise-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: Kubernetes service account or user bearer token presented to the API server.\n  sources:\n  - openapi/openkruise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openkruise/refs/heads/main/authentication/openkruise-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Native
- Controllers
- Deployment
- Incubating
- Kubernetes
- Workload Management
- CRDs
---
