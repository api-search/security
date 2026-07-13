---
api_key_in: []
api_specs:
- filename: microsoft-entra-graph-identity-openapi.yml
  format: yaml
  label: Microsoft Entra ID (Azure AD) API
  slug: graph-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/openapi/microsoft-entra-graph-identity-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Entra Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Entra secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Entra
provider_slug: microsoft-entra
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization using Microsoft identity platform. Supports authorization code flow for delegated permissions and client credentials flow for application permissions.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 12
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-entra-graph-identity-openapi.yml
  type: oauth2
slug: microsoft-entra-authentication
source_filename: microsoft-entra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-entra-graph-identity-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 12\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 1\n  description: OAuth 2.0 authorization using Microsoft identity platform. Supports authorization\n    code flow for delegated permissions and client credentials flow for application permissions.\n  sources:\n  - openapi/microsoft-entra-graph-identity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/authentication/microsoft-entra-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
---
