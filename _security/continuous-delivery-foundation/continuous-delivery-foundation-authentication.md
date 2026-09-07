---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml
  format: yaml
  label: Jenkins
  slug: jenkins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml
- filename: continuous-delivery-foundation-spinnaker-openapi.json
  format: json
  label: Spinnaker
  slug: spinnaker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-spinnaker-openapi.json
- filename: continuous-delivery-foundation-screwdriver-openapi.json
  format: json
  label: Screwdriver
  slug: screwdriver
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-screwdriver-openapi.json
- filename: continuous-delivery-foundation-jayex-jx-api-openapi.json
  format: json
  label: JayeX
  slug: jayex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/openapi/continuous-delivery-foundation-jayex-jx-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Continuous Delivery Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Continuous Delivery Foundation secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Continuous Delivery Foundation
provider_slug: continuous-delivery-foundation
scheme_count: 2
schemes:
- description: Jenkins basic authentication
  name: jenkins_auth
  scheme: basic
  sources:
  - openapi/continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml
  type: http
- in: header
  name: jwt
  parameter: Authorization
  sources:
  - openapi/continuous-delivery-foundation-screwdriver-openapi.json
  type: apiKey
slug: continuous-delivery-foundation-authentication
source_filename: continuous-delivery-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml, openapi/continuous-delivery-foundation-screwdriver-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: jenkins_auth\n  type: http\n  scheme: basic\n  description: Jenkins basic authentication\n  sources:\n  - openapi/continuous-delivery-foundation-jenkins-pipeline-graph-view-openapi.yaml\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/continuous-delivery-foundation-screwdriver-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/authentication/continuous-delivery-foundation-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Automation
- CI/CD
- DevOps
- Linux Foundation
- Open-Source
---
