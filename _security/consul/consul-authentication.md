---
api_key_in:
- header
api_specs:
- filename: consul-http-api.yml
  format: yaml
  label: Consul HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-http-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Consul Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Consul secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashiCorp Consul
provider_slug: consul
scheme_count: 1
schemes:
- description: ACL token for authentication
  in: header
  name: ConsulToken
  parameter: X-Consul-Token
  sources:
  - openapi/consul-http-api.yml
  type: apiKey
slug: consul-authentication
source_filename: consul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/consul-http-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ConsulToken\n  type: apiKey\n  in: header\n  parameter: X-Consul-Token\n  description: ACL token for authentication\n  sources:\n  - openapi/consul-http-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/authentication/consul-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ACL
- Configuration
- Health Checking
- Key/Value Store
- Multi-Datacenter
- Open Source
- Service Discovery
- Service Mesh
---
