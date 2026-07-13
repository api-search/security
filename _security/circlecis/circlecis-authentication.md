---
api_key_in:
- header
api_specs:
- filename: circlecis-openapi.yml
  format: yaml
  label: CircleCI REST API V2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/openapi/circlecis-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circlecis Authentication
name_suffix: Authentication
oauth_flows: []
overview: CircleCI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CircleCI
provider_slug: circlecis
scheme_count: 2
schemes:
- description: CircleCI personal API token.
  in: header
  name: apiTokenAuth
  parameter: Circle-Token
  sources:
  - openapi/circlecis-openapi.yml
  type: apiKey
- description: HTTP Basic with API token as username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/circlecis-openapi.yml
  type: http
slug: circlecis-authentication
source_filename: circlecis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circlecis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Circle-Token\n  description: CircleCI personal API token.\n  sources:\n  - openapi/circlecis-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with API token as username.\n  sources:\n  - openapi/circlecis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circlecis/refs/heads/main/authentication/circlecis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CI/CD
- Continuous Deployment
- Continuous Integration
- DevOps
- Pipelines
- Workflows
---
