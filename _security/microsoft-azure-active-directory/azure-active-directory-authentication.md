---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: microsoft-graph-identity-api.yml
  format: yaml
  label: Microsoft Graph Identity and Access API
  slug: microsoft-graph-identity-and-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/openapi/microsoft-graph-identity-api.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Active Directory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Azure Active Directory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
scheme_count: 1
schemes:
- description: Microsoft identity platform OAuth 2.0 authorization. Supports authorization code flow, client credentials flow, and on-behalf-of flow. All API calls require a valid access token obtained from the Microsoft identity platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 11
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-graph-identity-api.yml
  type: oauth2
slug: azure-active-directory-authentication
source_filename: azure-active-directory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-graph-identity-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 11\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft identity platform OAuth 2.0 authorization. Supports authorization code\n    flow, client credentials flow, and on-behalf-of flow. All API calls require a valid access\n    token obtained from the Microsoft identity platform.\n  sources:\n  - openapi/microsoft-graph-identity-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/authentication/azure-active-directory-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
---
