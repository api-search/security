---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Storsimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: StorSimple declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: StorSimple
provider_slug: storsimple
scheme_count: 1
schemes:
- authorization_endpoint: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize
  default_scope: https://management.azure.com/.default
  docs: https://learn.microsoft.com/en-us/rest/api/azure/
  flow: authorizationCode
  format: Bearer {token}
  header: Authorization
  name: azure_auth
  provider: Microsoft Entra ID (Azure AD)
  resource: https://management.azure.com/
  token_endpoint: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  transport: header
  type: oauth2
slug: storsimple-authentication
source_filename: storsimple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: Microsoft Learn - Azure StorSimple REST API reference (learn.microsoft.com/rest/api/storsimple)\nsummary: >-\n  The Azure StorSimple management REST API is an Azure Resource Manager (ARM) API. It\n  is authenticated with Microsoft Entra ID (Azure AD) OAuth 2.0 bearer tokens; every\n  request carries an Authorization: Bearer <token> header scoped to the Azure\n  subscription and the Microsoft.StorSimple resource provider.\nschemes:\n- type: oauth2\n  name: azure_auth\n  flow: authorizationCode\n  provider: Microsoft Entra ID (Azure AD)\n  token_endpoint: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n  authorization_endpoint: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize\n  resource: https://management.azure.com/\n  default_scope: https://management.azure.com/.default\n  transport: header\n  header: Authorization\n  format: Bearer {token}\n  docs: https://learn.microsoft.com/en-us/rest/api/azure/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storsimple/refs/heads/main/authentication/storsimple-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Storage
- Cloud Storage
- Hybrid Cloud
- Data Management
- Enterprise Storage
- Azure
- Acquired
---
