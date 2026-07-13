---
api_key_in:
- header
api_specs:
- filename: openapi
  format: yaml
  label: PHAIDRA Digital Collections REST API
  slug: phaidra
  spec_type: OpenAPI
  url: https://phaidra.cab.unipd.it/api/openapi
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Padua Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Padua secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Padua
provider_slug: university-of-padua
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/university-of-padua-phaidra.yaml
  type: http
- in: header
  name: tokenAuth
  parameter: X-XSRF-TOKEN
  sources:
  - openapi/university-of-padua-phaidra.yaml
  type: apiKey
slug: university-of-padua-authentication
source_filename: university-of-padua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-padua-phaidra.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-padua-phaidra.yaml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  sources:\n  - openapi/university-of-padua-phaidra.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/authentication/university-of-padua-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Library
- Repository
- Italy
---
