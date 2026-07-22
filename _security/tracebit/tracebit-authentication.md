---
api_key_in: []
api_specs:
- filename: tracebit-community-openapi-original.json
  format: json
  label: Tracebit API (Community Edition)
  slug: tracebit-api-community-edition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tracebit/refs/heads/main/openapi/tracebit-community-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tracebit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tracebit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tracebit
provider_slug: tracebit
scheme_count: 1
schemes:
- name: TracebitApiToken
  scheme: bearer
  sources:
  - openapi/tracebit-community-openapi-original.json
  type: http
slug: tracebit-authentication
source_filename: tracebit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tracebit-community-openapi-original.json\ndocs: https://community.tracebit.com/api-docs\nnotes: >-\n  The Tracebit API (Community Edition) authenticates with an API token sent as an\n  HTTP bearer token. API tokens are created in the Tracebit Community portal\n  (community.tracebit.com) and carry granular permissions referenced per operation\n  in the OpenAPI descriptions (e.g. canary-credentials:all:create, alerts:all:list,\n  alerts:all:get). The enterprise product docs (docs.tracebit.com) are\n  login-gated (HTTP 401). The host also publishes an OpenID Connect discovery\n  document at /.well-known/openid-configuration for its user login surface.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\npermissions:\n- permission: canary-credentials:all:create\n  operations:\n  - IssueCredentials\n  - ConfirmCredentials\n- permission: alerts:all:list\n  operations:\n  - ListAlerts\n\
  - permission: alerts:all:get\n  operations:\n  - GetAlertLogs\nschemes:\n- name: TracebitApiToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tracebit-community-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracebit/refs/heads/main/authentication/tracebit-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud Saas
- Security
- Deception
- Canary Tokens
- Threat Detection
- Cloud Security
- Incident Response
---
