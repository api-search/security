---
api_key_in:
- header
api_specs:
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey
  slug: portkey
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey Inference API
  slug: portkey-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey Admin API
  slug: portkey-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Portkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Portkey secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Portkey
provider_slug: portkey
scheme_count: 6
schemes:
- in: header
  name: Portkey-Key
  parameter: x-portkey-api-key
  sources:
  - openapi/portkey-openapi.yml
  type: apiKey
- in: header
  name: Virtual-Key
  parameter: x-portkey-virtual-key
  sources:
  - openapi/portkey-openapi.yml
  type: apiKey
- name: Provider-Auth
  scheme: bearer
  sources:
  - openapi/portkey-openapi.yml
  type: http
- in: header
  name: Provider-Name
  parameter: x-portkey-provider
  sources:
  - openapi/portkey-openapi.yml
  type: apiKey
- in: header
  name: Config
  parameter: x-portkey-config
  sources:
  - openapi/portkey-openapi.yml
  type: apiKey
- in: header
  name: Custom-Host
  parameter: x-portkey-custom-host
  sources:
  - openapi/portkey-openapi.yml
  type: apiKey
slug: portkey-authentication
source_filename: portkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portkey-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Portkey-Key\n  type: apiKey\n  in: header\n  parameter: x-portkey-api-key\n  sources:\n  - openapi/portkey-openapi.yml\n- name: Virtual-Key\n  type: apiKey\n  in: header\n  parameter: x-portkey-virtual-key\n  sources:\n  - openapi/portkey-openapi.yml\n- name: Provider-Auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/portkey-openapi.yml\n- name: Provider-Name\n  type: apiKey\n  in: header\n  parameter: x-portkey-provider\n  sources:\n  - openapi/portkey-openapi.yml\n- name: Config\n  type: apiKey\n  in: header\n  parameter: x-portkey-config\n  sources:\n  - openapi/portkey-openapi.yml\n- name: Custom-Host\n  type: apiKey\n  in: header\n  parameter: x-portkey-custom-host\n  sources:\n  - openapi/portkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/authentication/portkey-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- AI Gateways
- Gateways
- Governance
- Guardrails
- Observability
- Prompt Management
---
