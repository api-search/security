---
api_key_in: []
api_specs:
- filename: politecnico-di-torino-students-api.yaml
  format: yaml
  label: PoliTO REST API (api-spec)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-students-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Politecnico Di Torino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Politecnico di Torino secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Politecnico di Torino
provider_slug: politecnico-di-torino
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: Bearer
  sources:
  - openapi/politecnico-di-torino-faculty-api.yaml
  - openapi/politecnico-di-torino-students-api.yaml
  type: http
slug: politecnico-di-torino-authentication
source_filename: politecnico-di-torino-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/politecnico-di-torino-faculty-api.yaml, openapi/politecnico-di-torino-students-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: Bearer\n  sources:\n  - openapi/politecnico-di-torino-faculty-api.yaml\n  - openapi/politecnico-di-torino-students-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/authentication/politecnico-di-torino-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Italy
- Open Data
- Mobile
- OpenAPI
---
