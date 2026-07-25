---
api_key_in:
- query
api_specs:
- filename: nodeping-accounts-api-openapi.yml
  format: yaml
  label: NodePing Accounts API
  slug: nodeping-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-accounts-api-openapi.yml
- filename: nodeping-checks-api-openapi.yml
  format: yaml
  label: NodePing Checks API
  slug: nodeping-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-checks-api-openapi.yml
- filename: nodeping-contactgroups-api-openapi.yml
  format: yaml
  label: NodePing Contactgroups API
  slug: nodeping-contactgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-contactgroups-api-openapi.yml
- filename: nodeping-contacts-api-openapi.yml
  format: yaml
  label: NodePing Contacts API
  slug: nodeping-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-contacts-api-openapi.yml
- filename: nodeping-info-api-openapi.yml
  format: yaml
  label: NodePing Info API
  slug: nodeping-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-info-api-openapi.yml
- filename: nodeping-notifications-api-openapi.yml
  format: yaml
  label: NodePing Notifications API
  slug: nodeping-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-notifications-api-openapi.yml
- filename: nodeping-results-api-openapi.yml
  format: yaml
  label: NodePing Results API
  slug: nodeping-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-results-api-openapi.yml
- filename: nodeping-schedules-api-openapi.yml
  format: yaml
  label: NodePing Schedules API
  slug: nodeping-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/openapi/nodeping-schedules-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nodeping Authentication
name_suffix: Authentication
oauth_flows: []
overview: NodePing secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NodePing
provider_slug: nodeping
scheme_count: 2
schemes:
- description: API token passed as the `token` query parameter
  in: query
  name: ApiTokenQuery
  parameter: token
  sources:
  - openapi/nodeping-openapi.yml
  type: apiKey
- description: API token used as the username in HTTP Basic Auth
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/nodeping-openapi.yml
  type: http
slug: nodeping-authentication
source_filename: nodeping-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nodeping-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiTokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token passed as the `token` query parameter\n  sources:\n  - openapi/nodeping-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: API token used as the username in HTTP Basic Auth\n  sources:\n  - openapi/nodeping-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nodeping/refs/heads/main/authentication/nodeping-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Monitoring
- Uptime
- Notifications
- SaaS
---
