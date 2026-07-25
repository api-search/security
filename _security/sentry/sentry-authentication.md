---
api_key_in:
- header
api_specs:
- filename: sentry-webhooks-asyncapi.yml
  format: yaml
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/asyncapi/sentry-webhooks-asyncapi.yml
- filename: sentry-alerts-api-openapi.yml
  format: yaml
  label: Sentry Alerts API
  slug: sentry-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-alerts-api-openapi.yml
- filename: sentry-events-api-openapi.yml
  format: yaml
  label: Sentry Events API
  slug: sentry-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-events-api-openapi.yml
- filename: sentry-issues-api-openapi.yml
  format: yaml
  label: Sentry Issues API
  slug: sentry-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-issues-api-openapi.yml
- filename: sentry-organizations-api-openapi.yml
  format: yaml
  label: Sentry Organizations API
  slug: sentry-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-organizations-api-openapi.yml
- filename: sentry-projects-api-openapi.yml
  format: yaml
  label: Sentry Projects API
  slug: sentry-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-projects-api-openapi.yml
- filename: sentry-releases-api-openapi.yml
  format: yaml
  label: Sentry Releases API
  slug: sentry-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentry/refs/heads/main/openapi/sentry-releases-api-openapi.yml
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
