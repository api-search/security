---
api_key_in:
- header
- query
api_specs:
- filename: xsky-xms-swagger-original.yaml
  format: yaml
  label: XSKY XMS API
  slug: xsky-xms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xsky/refs/heads/main/openapi/xsky-xms-swagger-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Xsky Authentication
name_suffix: Authentication
oauth_flows: []
overview: XSKY secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: XSKY
provider_slug: xsky
scheme_count: 2
schemes:
- description: auth by token
  in: header
  name: tokenInHeader
  parameter: Xms-Auth-Token
  sources:
  - openapi/xsky-xms-swagger-original.yaml
  type: apiKey
- description: auth by token
  in: query
  name: tokenInQuery
  parameter: token
  sources:
  - openapi/xsky-xms-swagger-original.yaml
  type: apiKey
slug: xsky-authentication
source_filename: xsky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/xsky-xms-swagger-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: tokenInHeader\n  type: apiKey\n  in: header\n  parameter: Xms-Auth-Token\n  description: auth by token\n  sources:\n  - openapi/xsky-xms-swagger-original.yaml\n- name: tokenInQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: auth by token\n  sources:\n  - openapi/xsky-xms-swagger-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xsky/refs/heads/main/authentication/xsky-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Storage
- Software-Defined Storage
- Object Storage
- Block Storage
- File Storage
- Data Infrastructure
- Enterprise
- China
---
