---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Intune Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Intune secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Intune
provider_slug: microsoft-intune
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Azure Active Directory. Requires an active Intune license for the tenant.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-intune-openapi.yml
  type: oauth2
slug: microsoft-intune-authentication
source_filename: microsoft-intune-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-intune-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 4\n  description: OAuth 2.0 authorization using Azure Active Directory. Requires an active Intune\n    license for the tenant.\n  sources:\n  - openapi/microsoft-intune-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-intune/refs/heads/main/authentication/microsoft-intune-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- App Protection
- Azure
- Compliance
- Device Configuration
- Endpoint Management
- Enrollment
- MAM
- MDM
- Microsoft Graph
- Mobile Application Management
- Mobile Device Management
- Security
---
