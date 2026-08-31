---
api_key_in: []
api_specs:
- filename: choreo-alerts-api-openapi.yml
  format: yaml
  label: Choreo Alerts API
  slug: choreo-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-alerts-api-openapi.yml
- filename: choreo-apis-api-openapi.yml
  format: yaml
  label: Choreo Apis API
  slug: choreo-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-apis-api-openapi.yml
- filename: choreo-application-keys-api-openapi.yml
  format: yaml
  label: Choreo Application Keys API
  slug: choreo-application-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-application-keys-api-openapi.yml
- filename: choreo-applications-api-openapi.yml
  format: yaml
  label: Choreo Applications API
  slug: choreo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-applications-api-openapi.yml
- filename: choreo-builds-api-openapi.yml
  format: yaml
  label: Choreo Builds API
  slug: choreo-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-builds-api-openapi.yml
- filename: choreo-business-plans-api-openapi.yml
  format: yaml
  label: Choreo Business Plans API
  slug: choreo-business-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-business-plans-api-openapi.yml
- filename: choreo-components-api-openapi.yml
  format: yaml
  label: Choreo Components API
  slug: choreo-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-components-api-openapi.yml
- filename: choreo-deployments-api-openapi.yml
  format: yaml
  label: Choreo Deployments API
  slug: choreo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-deployments-api-openapi.yml
- filename: choreo-environments-api-openapi.yml
  format: yaml
  label: Choreo Environments API
  slug: choreo-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-environments-api-openapi.yml
- filename: choreo-errors-api-openapi.yml
  format: yaml
  label: Choreo Errors API
  slug: choreo-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-errors-api-openapi.yml
- filename: choreo-latency-api-openapi.yml
  format: yaml
  label: Choreo Latency API
  slug: choreo-latency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-latency-api-openapi.yml
- filename: choreo-logs-api-openapi.yml
  format: yaml
  label: Choreo Logs API
  slug: choreo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-logs-api-openapi.yml
- filename: choreo-organizations-api-openapi.yml
  format: yaml
  label: Choreo Organizations API
  slug: choreo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-organizations-api-openapi.yml
- filename: choreo-projects-api-openapi.yml
  format: yaml
  label: Choreo Projects API
  slug: choreo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-projects-api-openapi.yml
- filename: choreo-subscriptions-api-openapi.yml
  format: yaml
  label: Choreo Subscriptions API
  slug: choreo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-subscriptions-api-openapi.yml
- filename: choreo-usage-api-openapi.yml
  format: yaml
  label: Choreo Usage API
  slug: choreo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-usage-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Choreo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Choreo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Choreo
provider_slug: choreo
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://console.choreo.dev/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://console.choreo.dev/oauth2/token
  name: oauth2
  sources:
  - openapi/choreo-api-management-openapi.yml
  - openapi/choreo-developer-portal-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/choreo-api-management-openapi.yml
  - openapi/choreo-developer-portal-openapi.yml
  - openapi/choreo-insights-openapi.yml
  type: http
slug: choreo-authentication
source_filename: choreo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/choreo-api-management-openapi.yml, openapi/choreo-developer-portal-openapi.yml,\n  openapi/choreo-insights-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.choreo.dev/oauth2/authorize\n    tokenUrl: https://console.choreo.dev/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/choreo-api-management-openapi.yml\n  - openapi/choreo-developer-portal-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/choreo-api-management-openapi.yml\n  - openapi/choreo-developer-portal-openapi.yml\n  - openapi/choreo-insights-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/authentication/choreo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Apps
- API Management
- CI/CD
- Cloud-Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
---
