---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-stream-analytics-clusters-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Clusters API
  slug: microsoft-azure-stream-analytics-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-clusters-api-openapi.yml
- filename: microsoft-azure-stream-analytics-functions-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Functions API
  slug: microsoft-azure-stream-analytics-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-functions-api-openapi.yml
- filename: microsoft-azure-stream-analytics-inputs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Inputs API
  slug: microsoft-azure-stream-analytics-inputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-inputs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-outputs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Outputs API
  slug: microsoft-azure-stream-analytics-outputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-outputs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics StreamingJobs API
  slug: microsoft-azure-stream-analytics-streamingjobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
- filename: microsoft-azure-stream-analytics-transformations-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Transformations API
  slug: microsoft-azure-stream-analytics-transformations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-transformations-api-openapi.yml
- filename: microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Subscriptions API
  slug: microsoft-azure-stream-analytics-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
- filename: microsoft-azure-stream-analytics-operations-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Operations API
  slug: microsoft-azure-stream-analytics-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-operations-api-openapi.yml
- filename: microsoft-azure-stream-analytics-private-endpoints-api-openapi.yml
  format: yaml
  label: Azure Stream Analytics Private Endpoints API
  slug: microsoft-azure-stream-analytics-private-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-stream-analytics/openapi/microsoft-azure-stream-analytics-private-endpoints-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Azure Stream Analytics Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Stream Analytics secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Stream Analytics
provider_slug: microsoft-azure-stream-analytics
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/_superseded/microsoft-azure-stream-analytics-clusters-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-functions-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-inputs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-outputs-api-openapi.yml
  - openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml
  - openapi/_superseded/microsoft-azure-stream-analytics-transformations-api-openapi.yml
  type: oauth2
slug: microsoft-azure-stream-analytics-authentication
source_filename: microsoft-azure-stream-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/_superseded/microsoft-azure-stream-analytics-clusters-api-openapi.yml, openapi/_superseded/microsoft-azure-stream-analytics-functions-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-stream-analytics-inputs-api-openapi.yml, openapi/_superseded/microsoft-azure-stream-analytics-outputs-api-openapi.yml,\n  openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml, openapi/_superseded/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml, openapi/_superseded/microsoft-azure-stream-analytics-transformations-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow\n\
  \  sources:\n  - openapi/_superseded/microsoft-azure-stream-analytics-clusters-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-functions-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-inputs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-outputs-api-openapi.yml\n  - openapi/microsoft-azure-stream-analytics-privateendpoints-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-streamingjobs-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-subscriptions-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-stream-analytics-transformations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-stream-analytics/authentication/microsoft-azure-stream-analytics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Stream Processing
- Real-Time Analytics
- IoT
- Event Processing
- Microsoft Azure
- Streaming
---
