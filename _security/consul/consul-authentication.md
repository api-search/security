---
api_key_in:
- header
api_specs:
- filename: consul-acl-api-openapi.yml
  format: yaml
  label: HashiCorp Consul ACL API
  slug: consul-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-acl-api-openapi.yml
- filename: consul-agent-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Agent API
  slug: consul-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-agent-api-openapi.yml
- filename: consul-catalog-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Catalog API
  slug: consul-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-catalog-api-openapi.yml
- filename: consul-config-entries-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Config Entries API
  slug: consul-config-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-config-entries-api-openapi.yml
- filename: consul-connect-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Connect API
  slug: consul-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-connect-api-openapi.yml
- filename: consul-coordinates-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Coordinates API
  slug: consul-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-coordinates-api-openapi.yml
- filename: consul-events-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Events API
  slug: consul-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-events-api-openapi.yml
- filename: consul-health-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Health API
  slug: consul-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-health-api-openapi.yml
- filename: consul-kv-store-api-openapi.yml
  format: yaml
  label: HashiCorp Consul KV Store API
  slug: consul-kv-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-kv-store-api-openapi.yml
- filename: consul-operator-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Operator API
  slug: consul-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-operator-api-openapi.yml
- filename: consul-sessions-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Sessions API
  slug: consul-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-sessions-api-openapi.yml
- filename: consul-snapshot-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Snapshot API
  slug: consul-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-snapshot-api-openapi.yml
- filename: consul-status-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Status API
  slug: consul-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-status-api-openapi.yml
- filename: consul-transaction-api-openapi.yml
  format: yaml
  label: HashiCorp Consul Transaction API
  slug: consul-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-transaction-api-openapi.yml
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
- Open-Source
- Service Discovery
- Service Mesh
---
