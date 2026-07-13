---
api_key_in: []
api_specs:
- filename: microsoft-entra-id-openapi.yml
  format: yaml
  label: Microsoft Entra ID
  slug: microsoft-entra-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Entra Id Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Entra ID secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Entra ID
provider_slug: microsoft-entra-id
scheme_count: 1
schemes:
- description: Microsoft Entra ID OAuth 2.0 bearer token via Microsoft identity platform
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-entra-id-openapi.yml
  type: oauth2
slug: microsoft-entra-id-authentication
source_filename: microsoft-entra-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-entra-id-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 5\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token via Microsoft identity platform\n  sources:\n  - openapi/microsoft-entra-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/authentication/microsoft-entra-id-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Identity Provider
---
