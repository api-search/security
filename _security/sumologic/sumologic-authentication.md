---
api_key_in: []
api_specs:
- filename: sumologic-asyncapi.yml
  format: yaml
  label: Sumo Logic Webhook Connections
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumologic/refs/heads/main/asyncapi/sumologic-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sumologic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sumo Logic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sumo Logic
provider_slug: sumologic
scheme_count: 1
schemes:
- description: 'HTTP Basic Authentication. Use your Sumo Logic Access ID as username and

    the corresponding Access Key as password. Service account tokens may also

    be used. Generate credentials in the Sumo Logic UI under Administration

    > Security > Access Keys.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sumologic-openapi.yml
  type: http
slug: sumologic-authentication
source_filename: sumologic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sumologic-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Authentication. Use your Sumo Logic Access ID as username and\n    the corresponding Access Key as password. Service account tokens may also\n    be used. Generate credentials in the Sumo Logic UI under Administration\n    > Security > Access Keys.\n  sources:\n  - openapi/sumologic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumologic/refs/heads/main/authentication/sumologic-authentication.yml
summary_line: http · 1 scheme
tags:
- Logs
- Observability
- SIEM
- SOAR
- Metrics
- Cloud Security
- Log Analytics
---
