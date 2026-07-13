---
api_key_in: []
api_specs:
- filename: jenkins-openapi.yml
  format: yaml
  label: Jenkins Remote Access API
  slug: jenkins-remote-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jenkins Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jenkins secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jenkins
provider_slug: jenkins
scheme_count: 1
schemes:
- description: HTTP Basic auth using a Jenkins user and an API token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/jenkins-openapi.yml
  type: http
slug: jenkins-authentication
source_filename: jenkins-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jenkins-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using a Jenkins user and an API token.\n  sources:\n  - openapi/jenkins-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/authentication/jenkins-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Build Server
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Open Source
- Remote Access API
---
