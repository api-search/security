---
api_key_in: []
api_specs:
- filename: microsoft-active-directory-applications-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Applications API
  slug: microsoft-active-directory-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-applications-api-openapi.yml
- filename: microsoft-active-directory-directory-roles-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Directory Roles API
  slug: microsoft-active-directory-directory-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-directory-roles-api-openapi.yml
- filename: microsoft-active-directory-groups-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Groups API
  slug: microsoft-active-directory-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-groups-api-openapi.yml
- filename: microsoft-active-directory-service-principals-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Service Principals API
  slug: microsoft-active-directory-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-service-principals-api-openapi.yml
- filename: microsoft-active-directory-users-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Users API
  slug: microsoft-active-directory-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Active Directory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Active Directory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Active Directory
provider_slug: microsoft-active-directory
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-active-directory-openapi.yml
  type: oauth2
slug: microsoft-active-directory-authentication
source_filename: microsoft-active-directory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-active-directory-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 8\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-active-directory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/authentication/microsoft-active-directory-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Authorization
- Directory Services
- Enterprise
- Identity
- LDAP
- Windows
---
