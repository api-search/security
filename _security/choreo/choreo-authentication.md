---
api_key_in: []
api_specs:
- filename: choreo-api-management-openapi.yml
  format: yaml
  label: Choreo API Management API
  slug: api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-api-management-openapi.yml
- filename: choreo-developer-portal-openapi.yml
  format: yaml
  label: Choreo Developer Portal API
  slug: developer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-developer-portal-openapi.yml
- filename: choreo-insights-openapi.yml
  format: yaml
  label: Choreo Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-insights-openapi.yml
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
- Cloud Native
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
