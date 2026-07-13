---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Dataverse API (Common Data Service)
  slug: dataverse-api-common-data-service
  spec_type: OpenAPI
  url: https://docs.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Power Apps Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Power Apps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using Microsoft Entra ID (formerly Azure Active Directory). Applications must be registered in Microsoft Entra ID and granted appropriate Dataverse permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-power-apps-dataverse-web-api-openapi.yml
  type: oauth2
slug: microsoft-power-apps-authentication
source_filename: microsoft-power-apps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 2\n  description: OAuth 2.0 authentication using Microsoft Entra ID (formerly Azure Active Directory).\n    Applications must be registered in Microsoft Entra ID and granted appropriate Dataverse\n    permissions.\n  sources:\n  - openapi/microsoft-power-apps-dataverse-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/authentication/microsoft-power-apps-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
---
