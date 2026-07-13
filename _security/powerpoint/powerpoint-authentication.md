---
api_key_in: []
api_specs:
- filename: powerpoint-openapi.yml
  format: yaml
  label: PowerPoint via Microsoft Graph
  slug: powerpoint-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerpoint/refs/heads/main/openapi/powerpoint-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Powerpoint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PowerPoint secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PowerPoint
provider_slug: powerpoint
scheme_count: 1
schemes:
- description: 'Microsoft Graph uses Microsoft Entra ID (Azure AD) OAuth 2.0.

    Apps require delegated or application permissions such as Files.Read,

    Files.ReadWrite, Sites.Read.All, or Sites.ReadWrite.All.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: OAuth2
  sources:
  - openapi/powerpoint-openapi.yml
  type: oauth2
slug: powerpoint-authentication
source_filename: powerpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/powerpoint-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 4\n  description: |-\n    Microsoft Graph uses Microsoft Entra ID (Azure AD) OAuth 2.0.\n    Apps require delegated or application permissions such as Files.Read,\n    Files.ReadWrite, Sites.Read.All, or Sites.ReadWrite.All.\n  sources:\n  - openapi/powerpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerpoint/refs/heads/main/authentication/powerpoint-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Microsoft Office
- Microsoft 365
- Presentations
- Productivity
- Documents
---
