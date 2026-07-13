---
api_key_in:
- header
api_specs:
- filename: nuxeo-rest-api-openapi.yaml
  format: yaml
  label: Nuxeo REST API
  slug: nuxeo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuxeo/main/openapi/nuxeo-rest-api-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nuxeo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuxeo secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuxeo
provider_slug: nuxeo
scheme_count: 2
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/nuxeo-rest-api-openapi.yaml
  type: http
- in: header
  name: token
  parameter: X-Authentication-Token
  sources:
  - openapi/nuxeo-rest-api-openapi.yaml
  type: apiKey
slug: nuxeo-authentication
source_filename: nuxeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuxeo-rest-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/nuxeo-rest-api-openapi.yaml\n- name: token\n  type: apiKey\n  in: header\n  parameter: X-Authentication-Token\n  sources:\n  - openapi/nuxeo-rest-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuxeo/refs/heads/main/authentication/nuxeo-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Content Management
- Digital Asset Management
- Enterprise
- Documents
- Workflows
- Search
- Open Source
---
