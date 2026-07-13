---
api_key_in: []
api_specs:
- filename: heroku-platform-api.yml
  format: yaml
  label: Heroku Platform API
  slug: heroku-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-platform-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Heroku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heroku secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Heroku
provider_slug: heroku
scheme_count: 1
schemes:
- description: Heroku API key or OAuth token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/heroku-platform-api.yml
  type: http
slug: heroku-authentication
source_filename: heroku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heroku-platform-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Heroku API key or OAuth token\n  sources:\n  - openapi/heroku-platform-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/authentication/heroku-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Deployment
- Cloud Platform
- DevOps
- PaaS
---
