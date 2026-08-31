---
api_key_in: []
api_specs:
- filename: haproxy-data-plane-api-openapi.yml
  format: yaml
  label: HAProxy Data Plane API
  slug: haproxy-data-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haproxy/refs/heads/main/openapi/haproxy-data-plane-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Haproxy Authentication
name_suffix: Authentication
oauth_flows: []
overview: HAProxy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HAProxy
provider_slug: haproxy
scheme_count: 1
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/haproxy-data-plane-api-openapi.yml
  type: http
slug: haproxy-authentication
source_filename: haproxy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: derived\nsource: openapi/haproxy-data-plane-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/haproxy-data-plane-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haproxy/refs/heads/main/authentication/haproxy-authentication.yml
summary_line: http · 1 scheme
tags:
- High Availability
- Load Balancing
- Networking
- Reverse Proxy
- Proxy
- Kubernetes
- Ingress
- Open Source
- Infrastructure
- Application Delivery
---
