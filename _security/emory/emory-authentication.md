---
api_key_in:
- header
api_specs:
- filename: emory-digital-slide-archive.yaml
  format: yaml
  label: Emory Digital Slide Archive REST API
  slug: digital-slide-archive
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emory/refs/heads/main/openapi/emory-digital-slide-archive.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Emory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emory University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Emory University
provider_slug: emory
scheme_count: 1
schemes:
- in: header
  name: Girder-Token
  parameter: Girder-Token
  sources:
  - openapi/emory-digital-slide-archive.yaml
  type: apiKey
slug: emory-authentication
source_filename: emory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emory-digital-slide-archive.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Girder-Token\n  type: apiKey\n  in: header\n  parameter: Girder-Token\n  sources:\n  - openapi/emory-digital-slide-archive.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emory/refs/heads/main/authentication/emory-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Libraries
- United States
- Atlanta
---
