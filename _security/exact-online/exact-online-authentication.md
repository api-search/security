---
api_key_in: []
api_specs:
- filename: exact-online-openapi.yml
  format: yaml
  label: Exact Online REST / OData API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/openapi/exact-online-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Exact Online Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Exact Online secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Exact Online
provider_slug: exact-online
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://start.exactonline.nl/api/oauth2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://start.exactonline.nl/api/oauth2/token
  name: oauth2
  sources:
  - openapi/exact-online-openapi.yml
  type: oauth2
slug: exact-online-authentication
source_filename: exact-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/exact-online-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://start.exactonline.nl/api/oauth2/auth\n    tokenUrl: https://start.exactonline.nl/api/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/exact-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exact-online/refs/heads/main/authentication/exact-online-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Accounting
- ERP
- Invoicing
- Business Software
- CRM
- Financial Software
- SME
---
