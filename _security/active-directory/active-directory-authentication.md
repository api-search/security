---
api_key_in: []
api_specs:
- filename: active-directory-users-openapi.yaml
  format: yaml
  label: Microsoft Graph Users API
  slug: microsoft-graph-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-users-openapi.yaml
- filename: active-directory-groups-openapi.yaml
  format: yaml
  label: Microsoft Graph Groups API
  slug: microsoft-graph-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-groups-openapi.yaml
- filename: active-directory-applications-openapi.yaml
  format: yaml
  label: Microsoft Graph Applications and Service Principals API
  slug: microsoft-graph-applications-and-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-applications-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Active Directory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Active Directory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Active Directory
provider_slug: active-directory
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/active-directory-applications-openapi.yaml
  - openapi/active-directory-groups-openapi.yaml
  - openapi/active-directory-users-openapi.yaml
  type: oauth2
slug: active-directory-authentication
source_filename: active-directory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/active-directory-applications-openapi.yaml, openapi/active-directory-groups-openapi.yaml,\n  openapi/active-directory-users-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 2\n  sources:\n  - openapi/active-directory-applications-openapi.yaml\n  - openapi/active-directory-groups-openapi.yaml\n  - openapi/active-directory-users-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/authentication/active-directory-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
---
