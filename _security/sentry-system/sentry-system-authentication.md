---
api_key_in:
- header
api_specs:
- filename: openapi-derefed.json
  format: json
  label: Sentry API
  slug: sentry-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Events and Issues API
  slug: sentry-events-and-issues-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Organizations API
  slug: sentry-organizations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Projects API
  slug: sentry-projects-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Teams API
  slug: sentry-teams-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Releases API
  slug: sentry-releases-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Alerts API
  slug: sentry-alerts-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Crons API
  slug: sentry-crons-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Dashboards API
  slug: sentry-dashboards-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Discover API
  slug: sentry-discover-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Environments API
  slug: sentry-environments-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Explore API
  slug: sentry-explore-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integrations API
  slug: sentry-integrations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Mobile Builds API
  slug: sentry-mobile-builds-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Monitors API
  slug: sentry-monitors-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Prevent API
  slug: sentry-prevent-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Replays API
  slug: sentry-replays-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry SCIM API
  slug: sentry-scim-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Seer API
  slug: sentry-seer-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Users API
  slug: sentry-users-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sentry System Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentry secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sentry
provider_slug: sentry-system
scheme_count: 2
schemes:
- description: Authentication token for the Sentry API.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sentry-alerts-openapi.yml
  - openapi/sentry-api-openapi.yml
  - openapi/sentry-crons-openapi.yml
  - openapi/sentry-dashboards-openapi.yml
  - openapi/sentry-discover-openapi.yml
  - openapi/sentry-environments-openapi.yml
  - openapi/sentry-events-issues-openapi.yml
  - openapi/sentry-explore-openapi.yml
  - openapi/sentry-integration-platform-openapi.yml
  - openapi/sentry-integrations-openapi.yml
  - openapi/sentry-mobile-builds-openapi.yml
  - openapi/sentry-monitors-openapi.yml
  - openapi/sentry-organizations-openapi.yml
  - openapi/sentry-prevent-openapi.yml
  - openapi/sentry-projects-openapi.yml
  - openapi/sentry-releases-openapi.yml
  - openapi/sentry-replays-openapi.yml
  - openapi/sentry-scim-openapi.yml
  - openapi/sentry-seer-openapi.yml
  - openapi/sentry-teams-openapi.yml
  - openapi/sentry-users-openapi.yml
  type: http
- description: DSN-based authentication for event submission.
  in: header
  name: DSN
  parameter: X-Sentry-Auth
  sources:
  - openapi/sentry-api-openapi.yml
  type: apiKey
slug: sentry-system-authentication
source_filename: sentry-system-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sentry-alerts-openapi.yml, openapi/sentry-api-openapi.yml, openapi/sentry-crons-openapi.yml,\n  openapi/sentry-dashboards-openapi.yml, openapi/sentry-discover-openapi.yml, openapi/sentry-environments-openapi.yml,\n  openapi/sentry-events-issues-openapi.yml, openapi/sentry-explore-openapi.yml, openapi/sentry-integration-platform-openapi.yml,\n  openapi/sentry-integrations-openapi.yml, openapi/sentry-mobile-builds-openapi.yml, openapi/sentry-monitors-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authentication token for the Sentry API.\n  sources:\n  - openapi/sentry-alerts-openapi.yml\n  - openapi/sentry-api-openapi.yml\n  - openapi/sentry-crons-openapi.yml\n  - openapi/sentry-dashboards-openapi.yml\n  - openapi/sentry-discover-openapi.yml\n  - openapi/sentry-environments-openapi.yml\n  - openapi/sentry-events-issues-openapi.yml\n\
  \  - openapi/sentry-explore-openapi.yml\n  - openapi/sentry-integration-platform-openapi.yml\n  - openapi/sentry-integrations-openapi.yml\n  - openapi/sentry-mobile-builds-openapi.yml\n  - openapi/sentry-monitors-openapi.yml\n  - openapi/sentry-organizations-openapi.yml\n  - openapi/sentry-prevent-openapi.yml\n  - openapi/sentry-projects-openapi.yml\n  - openapi/sentry-releases-openapi.yml\n  - openapi/sentry-replays-openapi.yml\n  - openapi/sentry-scim-openapi.yml\n  - openapi/sentry-seer-openapi.yml\n  - openapi/sentry-teams-openapi.yml\n  - openapi/sentry-users-openapi.yml\n- name: DSN\n  type: apiKey\n  in: header\n  parameter: X-Sentry-Auth\n  description: DSN-based authentication for event submission.\n  sources:\n  - openapi/sentry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/authentication/sentry-system-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
---
