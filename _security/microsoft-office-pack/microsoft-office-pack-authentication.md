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
name: Microsoft Office Pack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft Office Pack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft Office Pack
provider_slug: microsoft-office-pack
scheme_count: 1
schemes:
- description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials, or device code flow depending on the scenario.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-office-pack-openapi.yml
  type: oauth2
slug: microsoft-office-pack-authentication
source_filename: microsoft-office-pack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-office-pack-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 7\n  description: Microsoft Entra ID (Azure AD) OAuth 2.0. Use the authorization code, client credentials,\n    or device code flow depending on the scenario.\n  sources:\n  - openapi/microsoft-office-pack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-pack/refs/heads/main/authentication/microsoft-office-pack-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
