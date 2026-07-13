---
api_key_in: []
api_specs:
- filename: microsoft-dynamics-365-sales-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API (Dynamics 365 Sales)
  slug: dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/openapi/microsoft-dynamics-365-sales-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Dynamics 365 Sales Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Dynamics 365 Sales secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Dynamics 365 Sales
provider_slug: microsoft-dynamics-365-sales
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-365-sales-openapi.yml
  type: oauth2
slug: microsoft-dynamics-365-sales-authentication
source_filename: microsoft-dynamics-365-sales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-sales-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n  sources:\n  - openapi/microsoft-dynamics-365-sales-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-sales/refs/heads/main/authentication/microsoft-dynamics-365-sales-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Customer Relationship Management
- Dynamics 365
- Microsoft
- Dataverse
- OData
- Sales Automation
---
