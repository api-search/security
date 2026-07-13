---
api_key_in:
- header
api_specs:
- filename: dynatrace-metrics-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Metrics API v2
  slug: dynatrace-metrics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-metrics-api-v2-openapi.yml
- filename: dynatrace-log-monitoring-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Log Monitoring API v2
  slug: dynatrace-log-monitoring-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-log-monitoring-api-v2-openapi.yml
- filename: dynatrace-account-management-api-openapi.yml
  format: yaml
  label: Dynatrace Account Management API
  slug: dynatrace-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-account-management-api-openapi.yml
- filename: dynatrace-events-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Events API v2
  slug: dynatrace-events-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-events-api-v2-openapi.yml
- filename: dynatrace-problems-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Problems API v2
  slug: dynatrace-problems-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-problems-api-v2-openapi.yml
- filename: dynatrace-entities-api-v2-openapi.yml
  format: yaml
  label: Dynatrace Entities API v2
  slug: dynatrace-entities-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/openapi/dynatrace-entities-api-v2-openapi.yml
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
- description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET operations, account-idm-write for POST/PUT/DELETE operations.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token
  name: oauth2
  sources:
  - openapi/dynatrace-account-management-api-openapi.yml
  type: oauth2
- description: 'Dynatrace API token. Use the format: Api-Token {your-token} Required scopes: entities.read'
  in: header
  name: api-token
  parameter: Authorization
  sources:
  - openapi/dynatrace-entities-api-v2-openapi.yml
  - openapi/dynatrace-events-api-v2-openapi.yml
  - openapi/dynatrace-log-monitoring-api-v2-openapi.yml
  - openapi/dynatrace-metrics-api-v2-openapi.yml
  - openapi/dynatrace-problems-api-v2-openapi.yml
  type: apiKey
slug: dynatrace-authentication
source_filename: dynatrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dynatrace-account-management-api-openapi.yml, openapi/dynatrace-entities-api-v2-openapi.yml,\n  openapi/dynatrace-events-api-v2-openapi.yml, openapi/dynatrace-log-monitoring-api-v2-openapi.yml,\n  openapi/dynatrace-metrics-api-v2-openapi.yml, openapi/dynatrace-problems-api-v2-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sso.dynatrace.com/sso/oauth2/token\n    scopes: 3\n  description: 'OAuth 2.0 authentication for the Account Management API. Use the client credentials\n    flow to obtain a bearer token. Required scopes vary by endpoint: account-idm-read for GET\n    operations, account-idm-write for POST/PUT/DELETE operations.'\n  sources:\n  - openapi/dynatrace-account-management-api-openapi.yml\n- name: api-token\n  type: apiKey\n  in:\
  \ header\n  parameter: Authorization\n  description: 'Dynatrace API token. Use the format: Api-Token {your-token} Required scopes:\n    entities.read'\n  sources:\n  - openapi/dynatrace-entities-api-v2-openapi.yml\n  - openapi/dynatrace-events-api-v2-openapi.yml\n  - openapi/dynatrace-log-monitoring-api-v2-openapi.yml\n  - openapi/dynatrace-metrics-api-v2-openapi.yml\n  - openapi/dynatrace-problems-api-v2-openapi.yml\n"
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
