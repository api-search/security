---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-advisor-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Operations API
  slug: microsoft-azure-advisor-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-operations-api-openapi.yml
- filename: microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Advisor Score Entities API
  slug: microsoft-azure-advisor-advisorscoreentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
- filename: microsoft-azure-advisor-metadataentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Metadata Entities API
  slug: microsoft-azure-advisor-metadataentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-metadataentities-api-openapi.yml
- filename: microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resiliency Reviews API
  slug: microsoft-azure-advisor-resiliencyreviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
- filename: microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resource Recommendation Bases API
  slug: microsoft-azure-advisor-resourcerecommendationbases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
- filename: microsoft-azure-advisor-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Subscriptions API
  slug: microsoft-azure-advisor-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-subscriptions-api-openapi.yml
- filename: microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Suppression Contracts API
  slug: microsoft-azure-advisor-suppressioncontracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Azure Advisor Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Azure Advisor secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Azure Advisor
provider_slug: microsoft-azure-advisor
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-advisor-openapi.yml
  - openapi/_superseded/microsoft-azure-advisor-operations-api-openapi.yml
  - openapi/_superseded/microsoft-azure-advisor-recommendations-api-openapi.yml
  type: oauth2
slug: microsoft-azure-advisor-authentication
source_filename: microsoft-azure-advisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-advisor-openapi.yml, openapi/_superseded/microsoft-azure-advisor-operations-api-openapi.yml,\n  openapi/_superseded/microsoft-azure-advisor-recommendations-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-advisor-openapi.yml\n  - openapi/_superseded/microsoft-azure-advisor-operations-api-openapi.yml\n  - openapi/_superseded/microsoft-azure-advisor-recommendations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-advisor/authentication/microsoft-azure-advisor-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advisor
- Best Practices
- Cost Optimization
- Microsoft Azure
- Optimization
- Recommendations
---
