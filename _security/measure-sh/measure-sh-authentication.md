---
anonymous_access: false
api_key_in: []
api_specs:
- filename: measure-sh-alerts-api-openapi.yml
  format: yaml
  label: Measure Alerts API
  slug: measure-sh-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-alerts-api-openapi.yml
- filename: measure-sh-apps-api-openapi.yml
  format: yaml
  label: Measure Apps API
  slug: measure-sh-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-apps-api-openapi.yml
- filename: measure-sh-auth-api-openapi.yml
  format: yaml
  label: Measure Auth API
  slug: measure-sh-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-auth-api-openapi.yml
- filename: measure-sh-bug-reports-api-openapi.yml
  format: yaml
  label: Measure Bug Reports API
  slug: measure-sh-bug-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-bug-reports-api-openapi.yml
- filename: measure-sh-builds-api-openapi.yml
  format: yaml
  label: Measure Builds API
  slug: measure-sh-builds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-builds-api-openapi.yml
- filename: measure-sh-config-api-openapi.yml
  format: yaml
  label: Measure Config API
  slug: measure-sh-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-config-api-openapi.yml
- filename: measure-sh-devices-api-openapi.yml
  format: yaml
  label: Measure Devices API
  slug: measure-sh-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-devices-api-openapi.yml
- filename: measure-sh-errors-api-openapi.yml
  format: yaml
  label: Measure Errors API
  slug: measure-sh-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-errors-api-openapi.yml
- filename: measure-sh-events-api-openapi.yml
  format: yaml
  label: Measure Events API
  slug: measure-sh-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-events-api-openapi.yml
- filename: measure-sh-funnels-api-openapi.yml
  format: yaml
  label: Measure Funnels API
  slug: measure-sh-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-funnels-api-openapi.yml
- filename: measure-sh-memory-api-openapi.yml
  format: yaml
  label: Measure Memory API
  slug: measure-sh-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-memory-api-openapi.yml
- filename: measure-sh-network-requests-api-openapi.yml
  format: yaml
  label: Measure Network Requests API
  slug: measure-sh-network-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-network-requests-api-openapi.yml
- filename: measure-sh-prefs-api-openapi.yml
  format: yaml
  label: Measure Prefs API
  slug: measure-sh-prefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-prefs-api-openapi.yml
- filename: measure-sh-profiles-api-openapi.yml
  format: yaml
  label: Measure Profiles API
  slug: measure-sh-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-profiles-api-openapi.yml
- filename: measure-sh-sessions-api-openapi.yml
  format: yaml
  label: Measure Sessions API
  slug: measure-sh-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-sessions-api-openapi.yml
- filename: measure-sh-teams-api-openapi.yml
  format: yaml
  label: Measure Teams API
  slug: measure-sh-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-teams-api-openapi.yml
- filename: measure-sh-traces-api-openapi.yml
  format: yaml
  label: Measure Traces API
  slug: measure-sh-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/measure-sh/openapi/measure-sh-traces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Measure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Measure declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Measure
provider_slug: measure-sh
scheme_count: 1
schemes:
- evidence: Authorization Copy Anchor Link bearerAuth header Authorization Bearer <JWT> User access token issued at sign-in.
  header: Authorization
  location: header
  name: bearerAuth
  type: http-bearer
slug: measure-sh-authentication
source_filename: measure-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://measure.sh/docs/api/dashboard/apps/rotateApiKey
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://measure.sh/docs/api/dashboard/apps/rotateApiKey\nsources:\n- https://measure.sh/docs/api/dashboard/apps/rotateApiKey\n- https://measure.sh/docs/hosting/google-oauth\n- https://measure.sh/docs/hosting/github-oauth\n- https://measure.sh/docs/api/dashboard/auth/getAuthSession\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: Authorization Copy Anchor Link bearerAuth header Authorization Bearer <JWT> User access token issued at sign-in.\n  location: header\n  header: Authorization\ndocs: https://measure.sh/docs/api/dashboard/apps/rotateApiKey\n"
source_yaml_url: https://artifacts.apis.io/measure-sh/authentication/measure-sh-authentication.yml
summary_line: 1 scheme
tags:
- Mobile
- Monitoring
- Open Source
- Crash Reporting
- Observability
---
