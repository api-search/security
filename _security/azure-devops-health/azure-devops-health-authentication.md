---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azure-devops-health-availabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Availability Statuses API
  slug: azure-devops-health-availabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-availabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childavailabilitystatuses-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Availability Statuses API
  slug: azure-devops-health-childavailabilitystatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml
- filename: azure-devops-health-childresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Child Resources API
  slug: azure-devops-health-childresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-childresources-api-openapi.yml
- filename: azure-devops-health-emergingissues-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Emerging Issues API
  slug: azure-devops-health-emergingissues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-emergingissues-api-openapi.yml
- filename: azure-devops-health-event-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event API
  slug: azure-devops-health-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-event-api-openapi.yml
- filename: azure-devops-health-eventimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Event Impacted Resources API
  slug: azure-devops-health-eventimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-eventimpactedresources-api-openapi.yml
- filename: azure-devops-health-events-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Events API
  slug: azure-devops-health-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-events-api-openapi.yml
- filename: azure-devops-health-metadata-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Metadata API
  slug: azure-devops-health-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-metadata-api-openapi.yml
- filename: azure-devops-health-operations-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Operations API
  slug: azure-devops-health-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-operations-api-openapi.yml
- filename: azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
  format: yaml
  label: Azure DevOps Health Security Advisory Impacted Resources API
  slug: azure-devops-health-securityadvisoryimpactedresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-devops-health/openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Azure Resource Health Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Resource Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Resource Health
provider_slug: azure-devops-health
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-devops-health-availabilitystatuses-api-openapi.yml
  - openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml
  - openapi/azure-devops-health-childresources-api-openapi.yml
  - openapi/azure-devops-health-emergingissues-api-openapi.yml
  - openapi/azure-devops-health-event-api-openapi.yml
  - openapi/azure-devops-health-eventimpactedresources-api-openapi.yml
  - openapi/azure-devops-health-events-api-openapi.yml
  - openapi/azure-devops-health-metadata-api-openapi.yml
  - openapi/azure-devops-health-operations-api-openapi.yml
  - openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml
  type: oauth2
slug: azure-devops-health-authentication
source_filename: azure-devops-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/azure-devops-health-availabilitystatuses-api-openapi.yml, openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml,\n  openapi/azure-devops-health-childresources-api-openapi.yml, openapi/azure-devops-health-emergingissues-api-openapi.yml,\n  openapi/azure-devops-health-event-api-openapi.yml, openapi/azure-devops-health-eventimpactedresources-api-openapi.yml,\n  openapi/azure-devops-health-events-api-openapi.yml, openapi/azure-devops-health-metadata-api-openapi.yml,\n  openapi/azure-devops-health-operations-api-openapi.yml, openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-devops-health-availabilitystatuses-api-openapi.yml\n\
  \  - openapi/azure-devops-health-childavailabilitystatuses-api-openapi.yml\n  - openapi/azure-devops-health-childresources-api-openapi.yml\n  - openapi/azure-devops-health-emergingissues-api-openapi.yml\n  - openapi/azure-devops-health-event-api-openapi.yml\n  - openapi/azure-devops-health-eventimpactedresources-api-openapi.yml\n  - openapi/azure-devops-health-events-api-openapi.yml\n  - openapi/azure-devops-health-metadata-api-openapi.yml\n  - openapi/azure-devops-health-operations-api-openapi.yml\n  - openapi/azure-devops-health-securityadvisoryimpactedresources-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-devops-health/authentication/azure-devops-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Continuous Integration
- Developer Tools
- Public APIs
- Microsoft Azure
- Microsoft
- Monitoring
- Service Health
---
