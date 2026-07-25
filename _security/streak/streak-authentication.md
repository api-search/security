---
api_key_in: []
api_specs:
- filename: streak-boxes-api-openapi.yml
  format: yaml
  label: Streak Boxes API
  slug: streak-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-boxes-api-openapi.yml
- filename: streak-fields-api-openapi.yml
  format: yaml
  label: Streak Fields API
  slug: streak-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-fields-api-openapi.yml
- filename: streak-newsfeed-api-openapi.yml
  format: yaml
  label: Streak Newsfeed API
  slug: streak-newsfeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-newsfeed-api-openapi.yml
- filename: streak-pipelines-api-openapi.yml
  format: yaml
  label: Streak Pipelines API
  slug: streak-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-pipelines-api-openapi.yml
- filename: streak-stages-api-openapi.yml
  format: yaml
  label: Streak Stages API
  slug: streak-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-stages-api-openapi.yml
- filename: streak-users-api-openapi.yml
  format: yaml
  label: Streak Users API
  slug: streak-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-users-api-openapi.yml
- filename: streak-webhooks-api-openapi.yml
  format: yaml
  label: Streak Webhooks API
  slug: streak-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streak/refs/heads/main/openapi/streak-webhooks-api-openapi.yml
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
