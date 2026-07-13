---
api_key_in:
- header
api_specs:
- filename: amazon-eventbridge-scheduler-openapi.yml
  format: yaml
  label: Amazon EventBridge Scheduler API
  slug: amazon-eventbridge-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/openapi/amazon-eventbridge-scheduler-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Eventbridge Scheduler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EventBridge Scheduler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-eventbridge-scheduler-openapi.yml
  type: apiKey
slug: amazon-eventbridge-scheduler-authentication
source_filename: amazon-eventbridge-scheduler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-eventbridge-scheduler-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-eventbridge-scheduler-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/authentication/amazon-eventbridge-scheduler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
---
