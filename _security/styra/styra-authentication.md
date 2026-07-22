---
api_key_in: []
api_specs:
- filename: styra-enterprise-opa-openapi.yaml
  format: yaml
  label: Styra Enterprise OPA / OPA REST API
  slug: styra-enterprise-opa-opa-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/styra/refs/heads/main/openapi/styra-enterprise-opa-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Styra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Styra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Styra
provider_slug: styra
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/styra-enterprise-opa-openapi.yaml
  type: http
slug: styra-authentication
source_filename: styra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/styra-enterprise-opa-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/styra-enterprise-opa-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/styra/refs/heads/main/authentication/styra-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Authorization
- Policy as Code
- Open Policy Agent
- Access Control
- Cloud Native
- API Security
---
