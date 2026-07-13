---
api_key_in: []
api_specs:
- filename: sharepoint-rest-openapi.json
  format: json
  label: SharePoint REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://example.com/sharepoint-rest-openapi.json
- filename: graph-sharepoint-openapi.json
  format: json
  label: Microsoft Graph API (SharePoint)
  slug: graph-api-sharepoint
  spec_type: OpenAPI
  url: https://example.com/graph-sharepoint-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sharepoint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft SharePoint secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft SharePoint
provider_slug: sharepoint
scheme_count: 1
schemes:
- description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/sharepoint-rest-api.yaml
  type: oauth2
slug: sharepoint-authentication
source_filename: sharepoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sharepoint-rest-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 4\n  description: OAuth 2.0 via Azure AD / Microsoft Identity Platform.\n  sources:\n  - openapi/sharepoint-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/authentication/sharepoint-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
---
