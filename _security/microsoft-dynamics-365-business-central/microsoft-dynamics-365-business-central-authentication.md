---
api_key_in: []
api_specs:
- filename: dynamics-open-api
  format: yaml
  label: Business Central API (v2.0)
  slug: api-v2
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/dynamics365/business-central/dev-itpro/api-reference/v2.0/dynamics-open-api
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Dynamics 365 Business Central Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Dynamics 365 Business Central secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Dynamics 365 Business Central
provider_slug: microsoft-dynamics-365-business-central
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-dynamics-365-business-central-openapi.yml
  type: oauth2
slug: microsoft-dynamics-365-business-central-authentication
source_filename: microsoft-dynamics-365-business-central-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-dynamics-365-business-central-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-dynamics-365-business-central-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365-business-central/refs/heads/main/authentication/microsoft-dynamics-365-business-central-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- ERP
- Cloud ERP
- Finance
- Accounting
- Supply Chain
- Operations
- Small Business
- Mid-Market
- Microsoft Dynamics 365
---
