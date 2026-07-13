---
api_key_in:
- header
api_specs:
- filename: inductive-automation-ignition-gateway.yaml
  format: yaml
  label: Ignition Gateway REST API
  slug: ignition-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inductive-automation/refs/heads/main/openapi/inductive-automation-ignition-gateway.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inductive Automation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inductive Automation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inductive Automation
provider_slug: inductive-automation
scheme_count: 1
schemes:
- description: Time-limited API token. Obtain by posting credentials to the token endpoint. See /data/api/v1/token for details.
  in: header
  name: apiKeyAuth
  parameter: X-Ignition-API-Token
  sources:
  - openapi/inductive-automation-ignition-gateway.yaml
  type: apiKey
slug: inductive-automation-authentication
source_filename: inductive-automation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/inductive-automation-ignition-gateway.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Ignition-API-Token\n  description: Time-limited API token. Obtain by posting credentials to the token endpoint.\n    See /data/api/v1/token for details.\n  sources:\n  - openapi/inductive-automation-ignition-gateway.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inductive-automation/refs/heads/main/authentication/inductive-automation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SCADA
- HMI
- Manufacturing
- IIoT
- Industrial Automation
- Industrial IoT
- OPC UA
---
