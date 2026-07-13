---
api_key_in:
- header
api_specs:
- filename: azure-log-analytics-query-api.yaml
  format: yaml
  label: Azure Log Analytics Query API
  slug: azure-log-analytics-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-query-api.yaml
- filename: azure-log-analytics-management-api.yaml
  format: yaml
  label: Azure Log Analytics Management API
  slug: azure-log-analytics-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-management-api.yaml
- filename: azure-log-analytics-ingestion-api.yaml
  format: yaml
  label: Azure Log Analytics Ingestion API
  slug: azure-log-analytics-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/openapi/azure-log-analytics-ingestion-api.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Log Analytics Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Log Analytics secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Microsoft Entra ID OAuth2 Bearer token obtained via client credentials flow. Use scope https://monitor.azure.com/.default for Azure public cloud.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/azure-log-analytics-ingestion-api.yaml
  - openapi/azure-log-analytics-query-api.yaml
  type: http
- description: Azure Active Directory OAuth2 implicit flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: oauth2
  sources:
  - openapi/azure-log-analytics-management-api.yaml
  type: oauth2
- description: API key authentication for the demo workspace only. Use DEMO_KEY with workspace ID DEMO_WORKSPACE for sample data exploration.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/azure-log-analytics-query-api.yaml
  type: apiKey
slug: azure-log-analytics-authentication
source_filename: azure-log-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-log-analytics-ingestion-api.yaml, openapi/azure-log-analytics-management-api.yaml,\n  openapi/azure-log-analytics-query-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Microsoft Entra ID OAuth2 Bearer token obtained via client credentials flow.\n    Use scope https://monitor.azure.com/.default for Azure public cloud.\n  sources:\n  - openapi/azure-log-analytics-ingestion-api.yaml\n  - openapi/azure-log-analytics-query-api.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 implicit flow.\n  sources:\n  - openapi/azure-log-analytics-management-api.yaml\n- name: apiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: X-Api-Key\n  description: API key authentication for the demo workspace only. Use DEMO_KEY with workspace\n    ID DEMO_WORKSPACE for sample data exploration.\n  sources:\n  - openapi/azure-log-analytics-query-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/authentication/azure-log-analytics-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
---
