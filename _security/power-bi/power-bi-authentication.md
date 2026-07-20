---
api_key_in: []
api_specs:
- filename: powerbi.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/powerbi/data-plane/Microsoft.PowerBI/stable/v1.0/powerbi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Power Bi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Power BI secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Power BI
provider_slug: power-bi
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Azure Active Directory / Microsoft Entra ID OAuth 2.0 access token. Register an Azure AD application, then request a token for the Power BI Service resource (https://analysis.windows.net/powerbi/api). Delegated (user) permissions use the authorization-code flow; app-only automation uses the client-credentials flow with the .default scope and requires tenant admin settings ("Allow service principals to use Power BI APIs").
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/power-bi-rest-api-openapi.yml
  type: http
slug: power-bi-authentication
source_filename: power-bi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/power-bi-rest-api-openapi.yml + Microsoft Power BI authentication docs\ndocs: https://learn.microsoft.com/en-us/power-bi/developer/embedded/get-azuread-access-token\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Azure Active Directory / Microsoft Entra ID OAuth 2.0 access token. Register\n    an Azure AD application, then request a token for the Power BI Service\n    resource (https://analysis.windows.net/powerbi/api). Delegated (user)\n    permissions use the authorization-code flow; app-only automation uses the\n    client-credentials flow with the .default scope and requires tenant admin\n    settings (\"Allow service principals to use Power BI APIs\").\n  sources:\n  - openapi/power-bi-rest-api-openapi.yml\nidentity_provider:\n  name: Microsoft Entra\
  \ ID (Azure AD)\n  authorize_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n  token_url: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  resource: https://analysis.windows.net/powerbi/api\nembed_tokens:\n  docs: https://learn.microsoft.com/en-us/power-bi/developer/embedded/embed-tokens\n  note: Embedded scenarios additionally mint short-lived Power BI embed tokens via GenerateToken for embed-for-your-customers and embed-for-your-organization.\nscopes_ref: scopes/power-bi-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/authentication/power-bi-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
---
