---
api_key_in:
- header
api_specs:
- filename: consul-connect-openapi.yml
  format: yaml
  label: Consul Connect HTTP API
  slug: consul-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/openapi/consul-connect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Consul Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consul Connect secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Consul Connect
provider_slug: consul-connect
scheme_count: 1
schemes:
- in: header
  name: ConsulToken
  parameter: X-Consul-Token
  sources:
  - openapi/consul-connect-openapi.yml
  type: apiKey
slug: consul-connect-authentication
source_filename: consul-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/consul-connect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ConsulToken\n  type: apiKey\n  in: header\n  parameter: X-Consul-Token\n  sources:\n  - openapi/consul-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consul-connect/refs/heads/main/authentication/consul-connect-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Consul
- Envoy
- HashiCorp
- Intentions
- Kubernetes
- mTLS
- Service Mesh
- Sidecar
- Zero Trust
---
