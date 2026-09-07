---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: datadog-apm-spans-api-openapi.yml
  format: yaml
  label: Datadog APM Spans API
  slug: datadog-apm-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-spans-api-openapi.yml
- filename: datadog-apm-spans-metrics-api-openapi.yml
  format: yaml
  label: Datadog APM Spans Metrics API
  slug: datadog-apm-spans-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-spans-metrics-api-openapi.yml
- filename: datadog-apm-retention-filters-api-openapi.yml
  format: yaml
  label: Datadog APM Retention Filters API
  slug: datadog-apm-retention-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-retention-filters-api-openapi.yml
- filename: datadog-apm-services-api-openapi.yml
  format: yaml
  label: Datadog APM Services API
  slug: datadog-apm-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-services-api-openapi.yml
- filename: datadog-apm-service-definitions-api-openapi.yml
  format: yaml
  label: Datadog APM Service Definitions API
  slug: datadog-apm-service-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-service-definitions-api-openapi.yml
- filename: datadog-apm-slos-api-openapi.yml
  format: yaml
  label: Datadog APM Service Level Objectives API
  slug: datadog-apm-slos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-slos-api-openapi.yml
- filename: datadog-apm-slo-corrections-api-openapi.yml
  format: yaml
  label: Datadog APM SLO Corrections API
  slug: datadog-apm-slo-corrections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/openapi/datadog-apm-slo-corrections-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Datadog Apm Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Datadog APM secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Datadog APM
provider_slug: datadog-apm
scheme_count: 6
schemes:
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: /oauth2/v1/authorize
    flow: authorizationCode
    scopes: 96
    tokenUrl: /oauth2/v1/token
  name: AuthZ
  sources:
  - openapi/datadog-apm-retention-filters-api-openapi.yml
  - openapi/datadog-apm-service-definitions-api-openapi.yml
  - openapi/datadog-apm-services-api-openapi.yml
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  - openapi/datadog-apm-spans-api-openapi.yml
  - openapi/datadog-apm-spans-metrics-api-openapi.yml
  type: oauth2
- description: Your Datadog API Key.
  in: header
  name: apiKeyAuth
  parameter: DD-API-KEY
  sources:
  - openapi/datadog-apm-retention-filters-api-openapi.yml
  - openapi/datadog-apm-service-definitions-api-openapi.yml
  - openapi/datadog-apm-services-api-openapi.yml
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  - openapi/datadog-apm-spans-api-openapi.yml
  - openapi/datadog-apm-spans-metrics-api-openapi.yml
  type: apiKey
- description: Your Datadog APP Key.
  in: header
  name: appKeyAuth
  parameter: DD-APPLICATION-KEY
  sources:
  - openapi/datadog-apm-retention-filters-api-openapi.yml
  - openapi/datadog-apm-service-definitions-api-openapi.yml
  - openapi/datadog-apm-services-api-openapi.yml
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  - openapi/datadog-apm-spans-api-openapi.yml
  - openapi/datadog-apm-spans-metrics-api-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datadog-apm-retention-filters-api-openapi.yml
  - openapi/datadog-apm-service-definitions-api-openapi.yml
  - openapi/datadog-apm-services-api-openapi.yml
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  - openapi/datadog-apm-spans-api-openapi.yml
  - openapi/datadog-apm-spans-metrics-api-openapi.yml
  type: http
- description: Deprecated API Key as query argument.
  in: query
  name: apiKeyAuthQuery
  parameter: api_key
  sources:
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  type: apiKey
- description: Deprecated APP Key as query argument.
  in: query
  name: appKeyAuthQuery
  parameter: application_key
  sources:
  - openapi/datadog-apm-slo-corrections-api-openapi.yml
  - openapi/datadog-apm-slos-api-openapi.yml
  type: apiKey
slug: datadog-apm-authentication
source_filename: datadog-apm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/datadog-apm-retention-filters-api-openapi.yml, openapi/datadog-apm-service-definitions-api-openapi.yml,\n  openapi/datadog-apm-services-api-openapi.yml, openapi/datadog-apm-slo-corrections-api-openapi.yml,\n  openapi/datadog-apm-slos-api-openapi.yml, openapi/datadog-apm-spans-api-openapi.yml, openapi/datadog-apm-spans-metrics-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AuthZ\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v1/authorize\n    tokenUrl: /oauth2/v1/token\n    scopes: 96\n  description: This API uses OAuth 2 with the implicit grant flow.\n  sources:\n  - openapi/datadog-apm-retention-filters-api-openapi.yml\n  - openapi/datadog-apm-service-definitions-api-openapi.yml\n  - openapi/datadog-apm-services-api-openapi.yml\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n\
  \  - openapi/datadog-apm-slos-api-openapi.yml\n  - openapi/datadog-apm-spans-api-openapi.yml\n  - openapi/datadog-apm-spans-metrics-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: DD-API-KEY\n  description: Your Datadog API Key.\n  sources:\n  - openapi/datadog-apm-retention-filters-api-openapi.yml\n  - openapi/datadog-apm-service-definitions-api-openapi.yml\n  - openapi/datadog-apm-services-api-openapi.yml\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n  - openapi/datadog-apm-slos-api-openapi.yml\n  - openapi/datadog-apm-spans-api-openapi.yml\n  - openapi/datadog-apm-spans-metrics-api-openapi.yml\n- name: appKeyAuth\n  type: apiKey\n  in: header\n  parameter: DD-APPLICATION-KEY\n  description: Your Datadog APP Key.\n  sources:\n  - openapi/datadog-apm-retention-filters-api-openapi.yml\n  - openapi/datadog-apm-service-definitions-api-openapi.yml\n  - openapi/datadog-apm-services-api-openapi.yml\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n\
  \  - openapi/datadog-apm-slos-api-openapi.yml\n  - openapi/datadog-apm-spans-api-openapi.yml\n  - openapi/datadog-apm-spans-metrics-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/datadog-apm-retention-filters-api-openapi.yml\n  - openapi/datadog-apm-service-definitions-api-openapi.yml\n  - openapi/datadog-apm-services-api-openapi.yml\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n  - openapi/datadog-apm-slos-api-openapi.yml\n  - openapi/datadog-apm-spans-api-openapi.yml\n  - openapi/datadog-apm-spans-metrics-api-openapi.yml\n- name: apiKeyAuthQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Deprecated API Key as query argument.\n  sources:\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n  - openapi/datadog-apm-slos-api-openapi.yml\n- name: appKeyAuthQuery\n  type: apiKey\n  in: query\n  parameter: application_key\n  description: Deprecated APP Key as query argument.\n  sources:\n  - openapi/datadog-apm-slo-corrections-api-openapi.yml\n\
  \  - openapi/datadog-apm-slos-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadog-apm/refs/heads/main/authentication/datadog-apm-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- APM
- Distributed Tracing
- Microservices
- Observability
- Performance Monitoring
- Spans
- Service Level Objectives
- Service Catalog
- OpenTelemetry
- MCP
---
