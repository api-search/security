---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-defender-for-cloud-datascanners-api-openapi.yml
  format: yaml
  label: Microsoft Defender for Cloud Data Scanners API
  slug: microsoft-defender-for-cloud-datascanners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-defender-for-cloud/openapi/microsoft-defender-for-cloud-datascanners-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Defender for Cloud Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Defender for Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Defender for Cloud
provider_slug: microsoft-defender-for-cloud
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/_superseded/microsoft-defender-for-cloud-alerts-api-openapi.yml
  - openapi/_superseded/microsoft-defender-for-cloud-assessments-api-openapi.yml
  - openapi/microsoft-defender-for-cloud-openapi.yml
  - openapi/_superseded/microsoft-defender-for-cloud-pricings-api-openapi.yml
  - openapi/_superseded/microsoft-defender-for-cloud-securescores-api-openapi.yml
  type: oauth2
slug: microsoft-defender-for-cloud-authentication
source_filename: microsoft-defender-for-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-defender-for-cloud-alerts-api-openapi.yml, openapi/_superseded/microsoft-defender-for-cloud-assessments-api-openapi.yml,\n  openapi/microsoft-defender-for-cloud-openapi.yml, openapi/_superseded/microsoft-defender-for-cloud-pricings-api-openapi.yml,\n  openapi/_superseded/microsoft-defender-for-cloud-securescores-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth 2.0\n  sources:\n  - openapi/_superseded/microsoft-defender-for-cloud-alerts-api-openapi.yml\n  - openapi/_superseded/microsoft-defender-for-cloud-assessments-api-openapi.yml\n  - openapi/microsoft-defender-for-cloud-openapi.yml\n  - openapi/_superseded/microsoft-defender-for-cloud-pricings-api-openapi.yml\n\
  \  - openapi/_superseded/microsoft-defender-for-cloud-securescores-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-defender-for-cloud/authentication/microsoft-defender-for-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Security
- CSPM
- CWPP
- CNAPP
- Threat Protection
- Compliance
- Vulnerability Management
- Microsoft Azure
---
