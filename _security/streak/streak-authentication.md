---
api_key_in: []
api_specs:
- filename: streak-openapi.yml
  format: yaml
  label: Streak REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Streak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Streak secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Streak
provider_slug: streak
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication. Set the username to your Streak API key and leave

    the password empty. Obtain an API key from

    https://support.streak.com/en/articles/2612883-get-your-streak-api-key.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/streak-openapi.yml
  type: http
slug: streak-authentication
source_filename: streak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streak-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication. Set the username to your Streak API key and leave\n    the password empty. Obtain an API key from\n    https://support.streak.com/en/articles/2612883-get-your-streak-api-key.\n  sources:\n  - openapi/streak-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/authentication/streak-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Sales
- Gmail
- Pipeline Management
- Email Tracking
- Productivity
- Small Business
- Workflow
---
