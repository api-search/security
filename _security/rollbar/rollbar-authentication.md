---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rollbar REST API
  slug: rollbar-rest-api
  spec_type: OpenAPI
  url: https://explorer.docs.rollbar.com/
- filename: rollbar-deployment-api-openapi.yml
  format: yaml
  label: Rollbar Deployment API
  slug: rollbar-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-deployment-api-openapi.yml
- filename: rollbar-metrics-api-openapi.yml
  format: yaml
  label: Rollbar Metrics API
  slug: rollbar-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-metrics-api-openapi.yml
- filename: rollbar-rql-api-openapi.yml
  format: yaml
  label: Rollbar RQL API
  slug: rollbar-rql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/openapi/rollbar-rql-api-openapi.yml
- filename: rollbar-webhooks-asyncapi.yml
  format: yaml
  label: Rollbar Webhooks
  slug: rollbar-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/asyncapi/rollbar-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rollbar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rollbar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rollbar
provider_slug: rollbar
scheme_count: 1
schemes:
- description: Rollbar access token for authentication. Requires write or post_server_item scope for creating deploys.
  in: header
  name: accessToken
  parameter: X-Rollbar-Access-Token
  sources:
  - openapi/rollbar-deployment-api-openapi.yml
  - openapi/rollbar-metrics-api-openapi.yml
  - openapi/rollbar-rest-api-openapi.yml
  - openapi/rollbar-rql-api-openapi.yml
  type: apiKey
slug: rollbar-authentication
source_filename: rollbar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rollbar-deployment-api-openapi.yml, openapi/rollbar-metrics-api-openapi.yml,\n  openapi/rollbar-rest-api-openapi.yml, openapi/rollbar-rql-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: X-Rollbar-Access-Token\n  description: Rollbar access token for authentication. Requires write or post_server_item scope\n    for creating deploys.\n  sources:\n  - openapi/rollbar-deployment-api-openapi.yml\n  - openapi/rollbar-metrics-api-openapi.yml\n  - openapi/rollbar-rest-api-openapi.yml\n  - openapi/rollbar-rql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollbar/refs/heads/main/authentication/rollbar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Error Tracking
- Monitoring
- Debugging
- DevOps
- Application Performance
---
