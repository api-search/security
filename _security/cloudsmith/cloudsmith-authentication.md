---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudsmith API (v1)
  slug: v1
  spec_type: OpenAPI
  url: https://api.cloudsmith.io/?format=openapi
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudsmith Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudsmith secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloudsmith
provider_slug: cloudsmith
scheme_count: 2
schemes:
- in: header
  name: apikey
  parameter: X-Api-Key
  sources:
  - openapi/cloudsmith-openapi.json
  type: apiKey
- name: basic
  scheme: basic
  sources:
  - openapi/cloudsmith-openapi.json
  type: http
slug: cloudsmith-authentication
source_filename: cloudsmith-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudsmith-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/cloudsmith-openapi.json\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cloudsmith-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsmith/refs/heads/main/authentication/cloudsmith-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artifact Management
- DevOps
- DevSecOps
- Distribution
- Package Management
- Registry
- Repository
- Software Supply Chain
- Universal
- Vulnerability Scanning
---
