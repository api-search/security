---
api_key_in: []
api_specs:
- filename: aflac-enterprise-connect-openapi.yml
  format: yaml
  label: Aflac Enterprise Connect API
  slug: enterprise-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-enterprise-connect-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aflac Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: aflac secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: aflac
provider_slug: aflac
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  sources:
  - openapi/aflac-enterprise-connect-openapi.yml
  type: oauth2
slug: aflac-authentication
source_filename: aflac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aflac-enterprise-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n    scopes: 6\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/authentication/aflac-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 500
---
