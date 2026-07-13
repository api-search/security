---
api_key_in: []
api_specs:
- filename: kuma-api-openapi.yml
  format: yaml
  label: Kuma API
  slug: kuma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/openapi/kuma-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kuma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kuma secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kuma
provider_slug: kuma
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/kuma-api-openapi.yml
  type: http
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kuma-api-openapi.yml
  type: http
slug: kuma-authentication
source_filename: kuma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kuma-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/kuma-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kuma-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuma/refs/heads/main/authentication/kuma-authentication.yml
summary_line: http · 2 schemes
tags:
- Envoy
- Kubernetes
- Microservices
- Security
- Service Mesh
---
