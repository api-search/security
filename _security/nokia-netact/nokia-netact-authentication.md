---
api_key_in: []
api_specs:
- filename: nokia-netact-nbi-openapi.yml
  format: yaml
  label: Nokia NetAct / Ericsson OSS API
  slug: nokia-netact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/openapi/nokia-netact-nbi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nokia Netact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nokia NetAct secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nokia NetAct
provider_slug: nokia-netact
scheme_count: 2
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nokia-netact-nbi-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/nokia-netact-nbi-openapi.yml
  type: http
slug: nokia-netact-authentication
source_filename: nokia-netact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nokia-netact-nbi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nokia-netact-nbi-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nokia-netact-nbi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/authentication/nokia-netact-authentication.yml
summary_line: http · 2 schemes
tags:
- Network Management
- OSS
- SNMP
- Telecom
---
