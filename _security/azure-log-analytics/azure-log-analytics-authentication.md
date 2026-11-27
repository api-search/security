---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: azure-log-analytics-tables-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Tables API
  slug: azure-log-analytics-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-tables-api-openapi.yml
- filename: azure-log-analytics-workspaces-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Workspaces API
  slug: azure-log-analytics-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-workspaces-api-openapi.yml
- filename: azure-log-analytics-availableservicetiers-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Available Service Tiers API
  slug: azure-log-analytics-availableservicetiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-availableservicetiers-api-openapi.yml
- filename: azure-log-analytics-clusters-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Clusters API
  slug: azure-log-analytics-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-clusters-api-openapi.yml
- filename: azure-log-analytics-deletedworkspaces-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Deleted Workspaces API
  slug: azure-log-analytics-deletedworkspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-deletedworkspaces-api-openapi.yml
- filename: azure-log-analytics-intelligencepacks-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Intelligence Packs API
  slug: azure-log-analytics-intelligencepacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-intelligencepacks-api-openapi.yml
- filename: azure-log-analytics-linkedservices-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Linked Services API
  slug: azure-log-analytics-linkedservices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-linkedservices-api-openapi.yml
- filename: azure-log-analytics-linkedstorageaccounts-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Linked Storage Accounts API
  slug: azure-log-analytics-linkedstorageaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-linkedstorageaccounts-api-openapi.yml
- filename: azure-log-analytics-networksecurityperimeterconfigurations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Network Security Perimeter Configurations API
  slug: azure-log-analytics-networksecurityperimeterconfigurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-networksecurityperimeterconfigurations-api-openapi.yml
- filename: azure-log-analytics-operations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Operations API
  slug: azure-log-analytics-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-operations-api-openapi.yml
- filename: azure-log-analytics-storageinsights-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Storage Insights API
  slug: azure-log-analytics-storageinsights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-storageinsights-api-openapi.yml
- filename: azure-log-analytics-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Subscriptions API
  slug: azure-log-analytics-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-subscriptions-api-openapi.yml
- filename: azure-log-analytics-summaryrules-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Summary Rules API
  slug: azure-log-analytics-summaryrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-summaryrules-api-openapi.yml
- filename: azure-log-analytics-async-operations-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Async Operations API
  slug: azure-log-analytics-async-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-async-operations-api-openapi.yml
- filename: azure-log-analytics-data-export-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Data Export API
  slug: azure-log-analytics-data-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-data-export-api-openapi.yml
- filename: azure-log-analytics-data-sources-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Data Sources API
  slug: azure-log-analytics-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-data-sources-api-openapi.yml
- filename: azure-log-analytics-saved-searches-api-openapi.yml
  format: yaml
  label: Azure Log Analytics Saved Searches API
  slug: azure-log-analytics-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-log-analytics/openapi/azure-log-analytics-saved-searches-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
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
source_yaml_url: https://artifacts.apis.io/azure-log-analytics/authentication/azure-log-analytics-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Analytics
- Microsoft Azure
- Cloud
- Logging
- Monitoring
---
