---
api_key_in: []
api_specs:
- filename: unum-hr-connect-openapi.yml
  format: yaml
  label: Unum HR Connect API
  slug: hr-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-hr-connect-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Unum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Unum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Unum
provider_slug: unum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api.unum.com/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/unum-hr-connect-openapi.yml
  type: oauth2
slug: unum-authentication
source_filename: unum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unum-hr-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.unum.com/v1/oauth/token\n    scopes: 9\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/authentication/unum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Insurance
- Benefits Administration
- HR Integration
- Disability Insurance
- Life Insurance
- Fortune 500
---
