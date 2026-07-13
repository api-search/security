---
api_key_in: []
api_specs:
- filename: teamcity-rest-api.yml
  format: yaml
  label: TeamCity REST API
  slug: teamcity-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-rest-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teamcity Authentication
name_suffix: Authentication
oauth_flows: []
overview: TeamCity secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TeamCity
provider_slug: teamcity
scheme_count: 2
schemes:
- description: Bearer token authentication using access tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teamcity-rest-api.yml
  type: http
- description: HTTP Basic authentication with username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/teamcity-rest-api.yml
  type: http
slug: teamcity-authentication
source_filename: teamcity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teamcity-rest-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using access tokens\n  sources:\n  - openapi/teamcity-rest-api.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with username and password\n  sources:\n  - openapi/teamcity-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/authentication/teamcity-authentication.yml
summary_line: http · 2 schemes
tags:
- Build Automation
- CI/CD
- Continuous Integration
- Deployment
- DevOps
- Testing
---
