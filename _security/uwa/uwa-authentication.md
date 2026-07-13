---
api_key_in:
- header
- query
api_specs:
- filename: uwa-research-repository.yaml
  format: yaml
  label: UWA Profiles and Research Repository (Pure CRIS Web Service)
  slug: research-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/openapi/uwa-research-repository.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uwa Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Western Australia secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Western Australia
provider_slug: uwa
scheme_count: 2
schemes:
- in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/uwa-research-repository.yaml
  type: apiKey
- in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/uwa-research-repository.yaml
  type: apiKey
slug: uwa-authentication
source_filename: uwa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uwa-research-repository.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/uwa-research-repository.yaml\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/uwa-research-repository.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/authentication/uwa-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Education
- Higher Education
- University
- Research
- Australia
- Perth
---
