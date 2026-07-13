---
api_key_in: []
api_specs:
- filename: $metadata
  format: yaml
  label: Dynamics 365 Sales API
  slug: dynamics-365-sales-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: $metadata
  format: yaml
  label: Dynamics 365 Customer Service API
  slug: dynamics-365-customer-service-api
  spec_type: OpenAPI
  url: https://[org].api.crm.dynamics.com/api/data/v9.2/$metadata
- filename: openapi
  format: yaml
  label: Dynamics 365 Business Central API
  slug: dynamics-365-business-central-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/dynamics365/business-central/dev-itpro/api-reference/v2.0/openapi
- filename: microsoft-dynamics-365-dataverse-web-api-openapi.yml
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Dynamics 365 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Dynamics 365 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Dynamics 365
provider_slug: microsoft-dynamics-365
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (Azure Active Directory). Applications must be registered in Microsoft Entra ID and granted the appropriate Dynamics 365 permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml
  type: oauth2
slug: microsoft-dynamics-365-authentication
source_filename: microsoft-dynamics-365-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authentication using Microsoft Entra ID (Azure Active Directory). Applications\n    must be registered in Microsoft Entra ID and granted the appropriate Dynamics 365 permissions.\n  sources:\n  - openapi/microsoft-dynamics-365-dataverse-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/authentication/microsoft-dynamics-365-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Applications
- Cloud
- CRM
- Enterprise
- ERP
- Microsoft
---
