---
api_key_in:
- header
api_specs:
- filename: openapi
  format: yaml
  label: PHAIDRA REST API
  slug: phaidra-api
  spec_type: OpenAPI
  url: https://services.phaidra.univie.ac.at/api/openapi
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Vienna Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Vienna secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Vienna
provider_slug: university-of-vienna
scheme_count: 2
schemes:
- in: header
  name: tokenAuth
  parameter: X-XSRF-TOKEN
  sources:
  - openapi/university-of-vienna-phaidra-api.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/university-of-vienna-phaidra-api.yaml
  type: http
slug: university-of-vienna-authentication
source_filename: university-of-vienna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-vienna-phaidra-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  sources:\n  - openapi/university-of-vienna-phaidra-api.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-vienna-phaidra-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/authentication/university-of-vienna-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Research
- Repository
- Open Data
- Austria
- Europe
---
