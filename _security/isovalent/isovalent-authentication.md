---
api_key_in: []
api_specs:
- filename: isovalent-cilium-agent-openapi.yml
  format: yaml
  label: Cilium Agent API
  slug: cilium-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/openapi/isovalent-cilium-agent-openapi.yml
- filename: isovalent-cilium-health-openapi.yml
  format: yaml
  label: Cilium Health API
  slug: cilium-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/openapi/isovalent-cilium-health-openapi.yml
auth_types:
- none-local-socket
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Isovalent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Isovalent secures its APIs with none-local-socket and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Isovalent
provider_slug: isovalent
scheme_count: 2
schemes:
- applies_to:
  - openapi/isovalent-cilium-agent-openapi.yml
  - openapi/isovalent-cilium-health-openapi.yml
  name: unix-socket
  scheme: local-unix-socket
  type: transport
- applies_to:
  - grpc/isovalent-hubble-observer.proto
  - grpc/isovalent-hubble-relay.proto
  docs: https://docs.cilium.io/en/stable/observability/hubble/configuration/tls/
  name: hubble-mtls
  scheme: mtls
  type: mutualTLS
slug: isovalent-authentication
source_filename: isovalent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.cilium.io/en/stable/security/\nsummary:\n  types: [none-local-socket, mutualTLS]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  The cilium-agent and cilium-health REST APIs declare no securityScheme in their\n  Swagger specs. Access control is enforced at the transport layer: the APIs are\n  served over local Unix domain sockets (unix:///var/run/cilium/cilium.sock and\n  .../health.sock) reachable only from within the agent's node/pod, not over the\n  network. The Hubble Observer/Relay gRPC APIs support optional mutual TLS (mTLS)\n  between Hubble peers and Relay, configured via Cilium's Hubble TLS settings, and\n  RBAC when exposed through Kubernetes. There is no API-key or OAuth surface.\nschemes:\n- name: unix-socket\n  type: transport\n  scheme: local-unix-socket\n  applies_to:\n  - openapi/isovalent-cilium-agent-openapi.yml\n  - openapi/isovalent-cilium-health-openapi.yml\n- name: hubble-mtls\n  type:\
  \ mutualTLS\n  scheme: mtls\n  docs: https://docs.cilium.io/en/stable/observability/hubble/configuration/tls/\n  applies_to:\n  - grpc/isovalent-hubble-observer.proto\n  - grpc/isovalent-hubble-relay.proto\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/authentication/isovalent-authentication.yml
summary_line: none-local-socket/mutualTLS · 2 schemes
tags:
- Company
- Networking
- Kubernetes
- eBPF
- Security
- Observability
- Cloud Native
- Service Mesh
- CNI
- Container Networking
---
