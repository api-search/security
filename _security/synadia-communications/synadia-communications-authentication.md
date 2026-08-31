---
api_key_in:
- cookie
- header
api_specs:
- filename: synadia-communications-control-plane-openapi.yaml
  format: yaml
  label: Synadia Control Plane / Synadia Cloud API
  slug: synadia-communications-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/openapi/synadia-communications-control-plane-openapi.yaml
- filename: synadia-communications-http-gateway-openapi.json
  format: json
  label: Synadia Cloud NATS HTTP Gateway
  slug: synadia-communications-http-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/openapi/synadia-communications-http-gateway-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synadia Communications Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synadia Communications secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Synadia Communications
provider_slug: synadia-communications
scheme_count: 3
schemes:
- bearerFormat: Personal Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synadia-communications-control-plane-openapi.yaml
  type: http
- in: cookie
  name: sessionAuth
  parameter: control_plane_session
  sources:
  - openapi/synadia-communications-control-plane-openapi.yaml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/synadia-communications-http-gateway-openapi.json
  type: apiKey
slug: synadia-communications-authentication
source_filename: synadia-communications-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/synadia-communications-control-plane-openapi.yaml, openapi/synadia-communications-http-gateway-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Personal Access Token\n  sources:\n  - openapi/synadia-communications-control-plane-openapi.yaml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: control_plane_session\n  sources:\n  - openapi/synadia-communications-control-plane-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/synadia-communications-http-gateway-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/authentication/synadia-communications-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Messaging
- Event Streaming
- NATS
- Distributed Systems
- Edge Computing
- Publish Subscribe
- Key-Value Store
- Object Storage
- Infrastructure
- Agentic AI
- Open-Source
---
