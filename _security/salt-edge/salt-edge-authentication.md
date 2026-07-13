---
api_key_in:
- header
api_specs:
- filename: salt-edge-openapi.yml
  format: yaml
  label: Salt Edge Account Information API
  slug: account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Salt Edge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salt Edge secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Salt Edge
provider_slug: salt-edge
scheme_count: 4
schemes:
- description: Salt Edge application identifier.
  in: header
  name: appId
  parameter: App-id
  sources:
  - openapi/salt-edge-openapi.yml
  type: apiKey
- description: Salt Edge application secret key.
  in: header
  name: secret
  parameter: Secret
  sources:
  - openapi/salt-edge-openapi.yml
  type: apiKey
- description: Base64-encoded SHA256 RSA signature (required in live mode).
  in: header
  name: signature
  parameter: Signature
  sources:
  - openapi/salt-edge-openapi.yml
  type: apiKey
- description: Unix-timestamp request expiration (required in live mode).
  in: header
  name: expiresAt
  parameter: Expires-at
  sources:
  - openapi/salt-edge-openapi.yml
  type: apiKey
slug: salt-edge-authentication
source_filename: salt-edge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salt-edge-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appId\n  type: apiKey\n  in: header\n  parameter: App-id\n  description: Salt Edge application identifier.\n  sources:\n  - openapi/salt-edge-openapi.yml\n- name: secret\n  type: apiKey\n  in: header\n  parameter: Secret\n  description: Salt Edge application secret key.\n  sources:\n  - openapi/salt-edge-openapi.yml\n- name: signature\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: Base64-encoded SHA256 RSA signature (required in live mode).\n  sources:\n  - openapi/salt-edge-openapi.yml\n- name: expiresAt\n  type: apiKey\n  in: header\n  parameter: Expires-at\n  description: Unix-timestamp request expiration (required in live mode).\n  sources:\n  - openapi/salt-edge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/authentication/salt-edge-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Fintech
- Open Banking
- PSD2
- Aggregator
- Global
- AISP
- PISP
- Compliance
- AML
---
