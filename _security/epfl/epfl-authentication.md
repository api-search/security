---
api_key_in:
- header
api_specs:
- filename: epfl-actu.yaml
  format: yaml
  label: EPFL Actu News API
  slug: actu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-actu.yaml
- filename: epfl-memento.yaml
  format: yaml
  label: EPFL Memento Events API
  slug: memento
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-memento.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Epfl Authentication
name_suffix: Authentication
oauth_flows: []
overview: EPFL secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EPFL
provider_slug: epfl
scheme_count: 2
schemes:
- description: 'DRF Token authentication, e.g. "Authorization: Token <key>".'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/epfl-actu.yaml
  - openapi/epfl-memento.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/epfl-actu.yaml
  - openapi/epfl-memento.yaml
  type: http
slug: epfl-authentication
source_filename: epfl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epfl-actu.yaml, openapi/epfl-memento.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'DRF Token authentication, e.g. \"Authorization: Token <key>\".'\n  sources:\n  - openapi/epfl-actu.yaml\n  - openapi/epfl-memento.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/epfl-actu.yaml\n  - openapi/epfl-memento.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/authentication/epfl-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Switzerland
- Europe
---
