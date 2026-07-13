---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: F5 Authentication
name_suffix: Authentication
oauth_flows: []
overview: F5 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: F5
provider_slug: f5
scheme_count: 2
schemes:
- description: HTTP Basic auth using a BIG-IP administrative user.
  name: Basic
  scheme: basic
  sources:
  - openapi/f5-openapi.yml
  type: http
- description: Token obtained from /mgmt/shared/authn/login.
  in: header
  name: Token
  parameter: X-F5-Auth-Token
  sources:
  - openapi/f5-openapi.yml
  type: apiKey
slug: f5-authentication
source_filename: f5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/f5-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using a BIG-IP administrative user.\n  sources:\n  - openapi/f5-openapi.yml\n- name: Token\n  type: apiKey\n  in: header\n  parameter: X-F5-Auth-Token\n  description: Token obtained from /mgmt/shared/authn/login.\n  sources:\n  - openapi/f5-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f5/refs/heads/main/authentication/f5-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Applications
- Security
- Load Balancing
- API Gateway
- WAF
---
