---
api_key_in:
- header
api_specs:
- filename: check-point-access-rules-api-openapi.yml
  format: yaml
  label: Check Point Software Access Rules API
  slug: check-point-access-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/openapi/check-point-access-rules-api-openapi.yml
- filename: check-point-gateways-api-openapi.yml
  format: yaml
  label: Check Point Software Gateways API
  slug: check-point-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/openapi/check-point-gateways-api-openapi.yml
- filename: check-point-hosts-api-openapi.yml
  format: yaml
  label: Check Point Software Hosts API
  slug: check-point-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/openapi/check-point-hosts-api-openapi.yml
- filename: check-point-networks-api-openapi.yml
  format: yaml
  label: Check Point Software Networks API
  slug: check-point-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/openapi/check-point-networks-api-openapi.yml
- filename: check-point-session-api-openapi.yml
  format: yaml
  label: Check Point Software Session API
  slug: check-point-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/openapi/check-point-session-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Check Point Authentication
name_suffix: Authentication
oauth_flows: []
overview: Check Point Software secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Check Point Software
provider_slug: check-point
scheme_count: 1
schemes:
- description: Session ID returned by /login, supplied on every subsequent call.
  in: header
  name: sessionId
  parameter: X-chkp-sid
  sources:
  - openapi/check-point-openapi.yml
  type: apiKey
slug: check-point-authentication
source_filename: check-point-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/check-point-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionId\n  type: apiKey\n  in: header\n  parameter: X-chkp-sid\n  description: Session ID returned by /login, supplied on every subsequent call.\n  sources:\n  - openapi/check-point-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/authentication/check-point-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Cybersecurity
- Firewall
- Network Security
- Cloud Security
- Endpoint Security
- Threat Intelligence
---
