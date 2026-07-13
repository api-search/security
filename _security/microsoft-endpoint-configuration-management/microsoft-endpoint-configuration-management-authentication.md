---
api_key_in: []
api_specs:
- filename: microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
  format: yaml
  label: Configuration Manager REST API
  slug: configuration-manager-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
  format: yaml
  label: Microsoft Intune Graph API
  slug: microsoft-intune-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
  format: yaml
  label: Intune Data Warehouse API
  slug: intune-data-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
- filename: microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
  format: yaml
  label: Intune Reporting Export API
  slug: intune-reporting-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Endpoint Configuration Management Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Endpoint Configuration Management secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
scheme_count: 2
schemes:
- description: Windows Integrated Authentication (Kerberos/NTLM).
  name: windowsAuth
  scheme: negotiate
  sources:
  - openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
  type: http
- description: OAuth 2.0 via Azure AD for cloud management gateway access.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml
  - openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml
  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml
  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml
  type: oauth2
slug: microsoft-endpoint-configuration-management-authentication
source_filename: microsoft-endpoint-configuration-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml,\n  openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml,\n  openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml, openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: windowsAuth\n  type: http\n  scheme: negotiate\n  description: Windows Integrated Authentication (Kerberos/NTLM).\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 0\n  description: OAuth\
  \ 2.0 via Azure AD for cloud management gateway access.\n  sources:\n  - openapi/microsoft-endpoint-configuration-management-configmgr-rest-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-data-warehouse-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-graph-api-openapi.yml\n  - openapi/microsoft-endpoint-configuration-management-intune-reporting-export-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/authentication/microsoft-endpoint-configuration-management-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
---
