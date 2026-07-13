---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudbees Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudBees secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudBees
provider_slug: cloudbees
scheme_count: 1
schemes:
- description: Jenkins username + API token
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cloudbees-openapi.yml
  type: http
slug: cloudbees-authentication
source_filename: cloudbees-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudbees-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Jenkins username + API token\n  sources:\n  - openapi/cloudbees-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/authentication/cloudbees-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Feature Flags
- Feature Management
- Jenkins
- Release Orchestration
- Software Delivery
---
