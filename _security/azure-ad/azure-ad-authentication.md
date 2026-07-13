---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Ad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Azure Active Directory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Azure Active Directory
provider_slug: azure-ad
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/azure-ad-openapi.yml
  type: oauth2
slug: azure-ad-authentication
source_filename: azure-ad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-ad-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 7\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/azure-ad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/authentication/azure-ad-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Authorization
- Identity
- OAuth
- OpenID Connect
- Single Sign-On
---
