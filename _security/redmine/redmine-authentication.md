---
api_key_in:
- header
- query
api_specs:
- filename: redmine-openapi.yml
  format: yaml
  label: Redmine REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/openapi/redmine-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Redmine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Redmine secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Redmine
provider_slug: redmine
scheme_count: 3
schemes:
- in: header
  name: apiKeyHeader
  parameter: X-Redmine-API-Key
  sources:
  - openapi/redmine-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/redmine-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/redmine-openapi.yml
  type: http
slug: redmine-authentication
source_filename: redmine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/redmine-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Redmine-API-Key\n  sources:\n  - openapi/redmine-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/redmine-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/redmine-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redmine/refs/heads/main/authentication/redmine-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Project Management
- Issue Tracking
- Open Source
- Ruby on Rails
- Bug Tracking
- Time Tracking
---
