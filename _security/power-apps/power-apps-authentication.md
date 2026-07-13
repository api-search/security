---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Power Apps REST API
  slug: power-apps-rest-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/connectors/powerappsforappmakers/
- filename: openapi
  format: yaml
  label: Microsoft Dataverse Web API
  slug: microsoft-dataverse-web-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/openapi
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Power Apps Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Power Apps secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Power Apps
provider_slug: power-apps
scheme_count: 1
schemes:
- description: 'Authentication uses Microsoft Entra ID (Azure AD) OAuth 2.0. Acquire a

    bearer token with the audience set to the Dataverse organization URL,

    for example https://{organization}.crm.dynamics.com/.default.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  sources:
  - openapi/power-apps-openapi.yml
  type: oauth2
slug: power-apps-authentication
source_filename: power-apps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/power-apps-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: |-\n    Authentication uses Microsoft Entra ID (Azure AD) OAuth 2.0. Acquire a\n    bearer token with the audience set to the Dataverse organization URL,\n    for example https://{organization}.crm.dynamics.com/.default.\n  sources:\n  - openapi/power-apps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-apps/refs/heads/main/authentication/power-apps-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- App Development
- Business Applications
- Cloud Platform
- Low-Code
- Microsoft
- No-Code
---
