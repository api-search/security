---
api_key_in: []
api_specs:
- filename: cloudbees-computer-api-openapi.yml
  format: yaml
  label: CloudBees Computer API
  slug: cloudbees-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-computer-api-openapi.yml
- filename: cloudbees-createitem-api-openapi.yml
  format: yaml
  label: CloudBees CreateItem API
  slug: cloudbees-createitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-createitem-api-openapi.yml
- filename: cloudbees-job-api-openapi.yml
  format: yaml
  label: CloudBees Job API
  slug: cloudbees-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-job-api-openapi.yml
- filename: cloudbees-json-api-openapi.yml
  format: yaml
  label: CloudBees Json API
  slug: cloudbees-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-json-api-openapi.yml
- filename: cloudbees-python-api-openapi.yml
  format: yaml
  label: CloudBees Python API
  slug: cloudbees-python-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-python-api-openapi.yml
- filename: cloudbees-queue-api-openapi.yml
  format: yaml
  label: CloudBees Queue API
  slug: cloudbees-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-queue-api-openapi.yml
- filename: cloudbees-xml-api-openapi.yml
  format: yaml
  label: CloudBees Xml API
  slug: cloudbees-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-xml-api-openapi.yml
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
