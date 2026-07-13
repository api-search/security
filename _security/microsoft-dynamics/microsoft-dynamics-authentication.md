---
api_key_in: []
api_specs:
- filename: microsoft-dynamics-business-central-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Business Central API
  slug: business-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-business-central-openapi.yml
- filename: microsoft-dynamics-dataverse-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Dataverse Web API
  slug: dataverse-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-dataverse-openapi.yml
- filename: microsoft-dynamics-finance-operations-openapi.yml
  format: yaml
  label: Microsoft Dynamics 365 Finance & Operations Data API
  slug: finance-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/openapi/microsoft-dynamics-finance-operations-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Dynamics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Dynamics secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
scheme_count: 2
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-business-central-openapi.yml
  - openapi/microsoft-dynamics-dataverse-openapi.yml
  type: oauth2
- description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-finance-operations-openapi.yml
  type: oauth2
slug: microsoft-dynamics-authentication
source_filename: microsoft-dynamics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-business-central-openapi.yml, openapi/microsoft-dynamics-dataverse-openapi.yml,\n  openapi/microsoft-dynamics-finance-operations-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0 authentication.\n  sources:\n  - openapi/microsoft-dynamics-business-central-openapi.yml\n  - openapi/microsoft-dynamics-dataverse-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0\
  \ authentication.\n  sources:\n  - openapi/microsoft-dynamics-finance-operations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/authentication/microsoft-dynamics-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- CRM
- ERP
- Microsoft Dynamics
---
