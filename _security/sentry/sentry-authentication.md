---
api_key_in:
- header
api_specs:
- filename: sentry-api-openapi.yml
  format: yaml
  label: Sentry Error Monitoring API
  slug: sentry-error-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-api-openapi.yml
- filename: sentry-webhooks-asyncapi.yml
  format: yaml
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/asyncapi/sentry-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sentry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentry secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sentry
provider_slug: sentry
scheme_count: 2
schemes:
- description: 'Format: Token YOUR_AUTH_TOKEN'
  in: header
  name: AuthToken
  parameter: Authorization
  sources:
  - openapi/sentry-api-openapi.yml
  type: apiKey
- description: OAuth2 Bearer token for integrations
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sentry-api-openapi.yml
  type: http
slug: sentry-authentication
source_filename: sentry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sentry-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AuthToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Format: Token YOUR_AUTH_TOKEN'\n  sources:\n  - openapi/sentry-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer token for integrations\n  sources:\n  - openapi/sentry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/authentication/sentry-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Error Monitoring
- Debugging
- Observability
- Application Performance Management
- Developer Tools
---
