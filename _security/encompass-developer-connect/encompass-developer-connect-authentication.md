---
api_key_in: []
api_specs:
- filename: encompass-developer-connect-openapi.yml
  format: yaml
  label: Encompass Developer Connect API
  slug: encompass-developer-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass-developer-connect/refs/heads/main/openapi/encompass-developer-connect-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Encompass Developer Connect Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Encompass Developer Connect secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Encompass Developer Connect
provider_slug: encompass-developer-connect
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/encompass-developer-connect-openapi.yml
  type: oauth2
slug: encompass-developer-connect-authentication
source_filename: encompass-developer-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/encompass-developer-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\n    scopes: 2\n  sources:\n  - openapi/encompass-developer-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass-developer-connect/refs/heads/main/authentication/encompass-developer-connect-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Encompass
- ICE Mortgage Technology
- Loan Origination
- Lending
- Mortgage
- REST API
---
