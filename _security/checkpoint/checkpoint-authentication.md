---
api_key_in:
- header
api_specs:
- filename: checkpoint-management-api-openapi.yml
  format: yaml
  label: Check Point Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-management-api-openapi.yml
- filename: checkpoint-gaia-api-openapi.yml
  format: yaml
  label: Check Point Gaia API
  slug: gaia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-gaia-api-openapi.yml
- filename: checkpoint-cloudguard-api-openapi.yml
  format: yaml
  label: Check Point CloudGuard API
  slug: cloudguard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-cloudguard-api-openapi.yml
- filename: checkpoint-identity-awareness-api-openapi.yml
  format: yaml
  label: Check Point Identity Awareness API
  slug: identity-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-identity-awareness-api-openapi.yml
- filename: checkpoint-harmony-email-api-openapi.yml
  format: yaml
  label: Check Point Harmony Email API
  slug: harmony-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-harmony-email-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Check Point secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Check Point
provider_slug: checkpoint
scheme_count: 4
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/checkpoint-cloudguard-api-openapi.yml
  type: http
- in: header
  name: sidToken
  parameter: X-chkp-sid
  sources:
  - openapi/checkpoint-gaia-api-openapi.yml
  - openapi/checkpoint-management-api-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkpoint-harmony-email-api-openapi.yml
  type: http
- in: header
  name: sharedSecret
  parameter: X-chkp-shared-secret
  sources:
  - openapi/checkpoint-identity-awareness-api-openapi.yml
  type: apiKey
slug: checkpoint-authentication
source_filename: checkpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkpoint-cloudguard-api-openapi.yml, openapi/checkpoint-gaia-api-openapi.yml,\n  openapi/checkpoint-harmony-email-api-openapi.yml, openapi/checkpoint-identity-awareness-api-openapi.yml,\n  openapi/checkpoint-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/checkpoint-cloudguard-api-openapi.yml\n- name: sidToken\n  type: apiKey\n  in: header\n  parameter: X-chkp-sid\n  sources:\n  - openapi/checkpoint-gaia-api-openapi.yml\n  - openapi/checkpoint-management-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/checkpoint-harmony-email-api-openapi.yml\n- name: sharedSecret\n  type: apiKey\n  in: header\n  parameter: X-chkp-shared-secret\n  sources:\n  - openapi/checkpoint-identity-awareness-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/authentication/checkpoint-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Firewall
- Identity Awareness
- Mobile Security
- Network Security
- Security
- Threat Prevention
- WAF
---
