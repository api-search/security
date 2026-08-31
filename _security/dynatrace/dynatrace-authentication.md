---
api_key_in:
- header
api_specs:
- filename: dynatrace-entities-api-openapi.yml
  format: yaml
  label: Dynatrace Entities API
  slug: dynatrace-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-entities-api-openapi.yml
- filename: dynatrace-environments-api-openapi.yml
  format: yaml
  label: Dynatrace Environments API
  slug: dynatrace-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-environments-api-openapi.yml
- filename: dynatrace-events-api-openapi.yml
  format: yaml
  label: Dynatrace Events API
  slug: dynatrace-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-events-api-openapi.yml
- filename: dynatrace-groups-api-openapi.yml
  format: yaml
  label: Dynatrace Groups API
  slug: dynatrace-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-groups-api-openapi.yml
- filename: dynatrace-logs-api-openapi.yml
  format: yaml
  label: Dynatrace Logs API
  slug: dynatrace-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-logs-api-openapi.yml
- filename: dynatrace-metrics-api-openapi.yml
  format: yaml
  label: Dynatrace Metrics API
  slug: dynatrace-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-metrics-api-openapi.yml
- filename: dynatrace-permissions-api-openapi.yml
  format: yaml
  label: Dynatrace Permissions API
  slug: dynatrace-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-permissions-api-openapi.yml
- filename: dynatrace-problems-api-openapi.yml
  format: yaml
  label: Dynatrace Problems API
  slug: dynatrace-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-problems-api-openapi.yml
- filename: dynatrace-users-api-openapi.yml
  format: yaml
  label: Dynatrace Users API
  slug: dynatrace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dynatrace Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Dynatrace secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Dynatrace
provider_slug: dynatrace
scheme_count: 2
schemes:
- description: 'Dynatrace API token. Use the format: Api-Token {your-token} Required scopes: entities.read'
  in: header
  name: api-token
  parameter: Authorization
  sources:
  - openapi/dynatrace-entities-api-openapi.yml
  - openapi/dynatrace-events-api-openapi.yml
  - openapi/dynatrace-logs-api-openapi.yml
  - openapi/dynatrace-metrics-api-openapi.yml
  - openapi/dynatrace-problems-api-openapi.yml
  type: apiKey
- description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET operations, account-idm-write for POST/PUT/DELETE operations.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token
  name: oauth2
  sources:
  - openapi/dynatrace-environments-api-openapi.yml
  - openapi/dynatrace-groups-api-openapi.yml
  - openapi/dynatrace-permissions-api-openapi.yml
  - openapi/dynatrace-users-api-openapi.yml
  type: oauth2
slug: dynatrace-authentication
source_filename: dynatrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/dynatrace-entities-api-openapi.yml, openapi/dynatrace-environments-api-openapi.yml,\n  openapi/dynatrace-events-api-openapi.yml, openapi/dynatrace-groups-api-openapi.yml, openapi/dynatrace-logs-api-openapi.yml,\n  openapi/dynatrace-metrics-api-openapi.yml, openapi/dynatrace-permissions-api-openapi.yml,\n  openapi/dynatrace-problems-api-openapi.yml, openapi/dynatrace-users-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: api-token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Dynatrace API token. Use the format: Api-Token {your-token} Required scopes:\n    entities.read'\n  sources:\n  - openapi/dynatrace-entities-api-openapi.yml\n  - openapi/dynatrace-events-api-openapi.yml\n  - openapi/dynatrace-logs-api-openapi.yml\n  - openapi/dynatrace-metrics-api-openapi.yml\n  - openapi/dynatrace-problems-api-openapi.yml\n\
  - name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token\n    scopes: 3\n  description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials\n    flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET\n    operations, account-idm-write for POST/PUT/DELETE operations.'\n  sources:\n  - openapi/dynatrace-environments-api-openapi.yml\n  - openapi/dynatrace-groups-api-openapi.yml\n  - openapi/dynatrace-permissions-api-openapi.yml\n  - openapi/dynatrace-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/authentication/dynatrace-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
---
