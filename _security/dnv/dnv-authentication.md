---
api_key_in: []
api_specs:
- filename: dnv-class-status-openapi.yml
  format: yaml
  label: DNV Class Status API
  slug: dnv-class-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/openapi/dnv-class-status-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dnv Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: DNV secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: DNV
provider_slug: dnv
scheme_count: 1
schemes:
- description: OAuth 2.0 via Azure AD B2C. Tokens obtained from https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token using client credentials grant with resource ID c916a223-f3d4-4d43-b709-cfcd77ff4a05.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token
  name: oauth2
  sources:
  - openapi/dnv-class-status-openapi.yml
  type: oauth2
slug: dnv-authentication
source_filename: dnv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dnv-class-status-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 via Azure AD B2C. Tokens obtained from https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token\n    using client credentials grant with resource ID c916a223-f3d4-4d43-b709-cfcd77ff4a05.\n  sources:\n  - openapi/dnv-class-status-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/authentication/dnv-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Maritime
- Energy
- Classification
- Vessel
- Data Platform
---
