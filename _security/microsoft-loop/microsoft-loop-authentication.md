---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-loop-storage-filestorage-api-openapi.yml
  format: yaml
  label: Microsoft Loop Storage.file Storage API
  slug: microsoft-loop-storage-filestorage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-loop/openapi/microsoft-loop-storage-filestorage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Microsoft Loop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Loop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Microsoft Loop
provider_slug: microsoft-loop
scheme_count: 1
schemes:
- authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
  description: Loop workspaces are reached through Microsoft Graph; every call needs an access token issued by the Microsoft identity platform (delegated or application permissions).
  header: 'Authorization: Bearer <token>'
  name: Microsoft identity platform (Microsoft Entra ID)
  tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  type: oauth2
slug: microsoft-loop-authentication
source_filename: microsoft-loop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Microsoft Loop authentication\ngenerated: '2026-11-12'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/graph/auth/\ndocs: https://learn.microsoft.com/en-us/graph/auth/\nschemes:\n  - type: oauth2\n    name: Microsoft identity platform (Microsoft Entra ID)\n    description: Loop workspaces are reached through Microsoft Graph; every call needs an access token issued by the Microsoft identity platform (delegated or application permissions).\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    authorizationUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n    header: 'Authorization: Bearer <token>'\n"
source_yaml_url: https://artifacts.apis.io/microsoft-loop/authentication/microsoft-loop-authentication.yml
summary_line: 1 scheme
tags:
- Collaboration
- Microsoft
- Microsoft 365
- Productivity
- Workspace
---
