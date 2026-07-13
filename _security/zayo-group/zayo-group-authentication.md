---
api_key_in: []
api_specs:
- filename: zayo-group-openapi.yml
  format: yaml
  label: Zayo Group Holdings API
  slug: zayo-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo-group/refs/heads/main/openapi/zayo-group-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zayo Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zayo Group Holdings secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zayo Group Holdings
provider_slug: zayo-group
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant. Exchange client_id / client_secret at

    the authorization server token endpoint for a short-lived bearer token

    (tokens expire hourly).'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.api.zayo.com/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/zayo-group-openapi.yml
  type: oauth2
slug: zayo-group-authentication
source_filename: zayo-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zayo-group-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.zayo.com/oauth/token\n    scopes: 0\n  description: |-\n    OAuth 2.0 Client Credentials grant. Exchange client_id / client_secret at\n    the authorization server token endpoint for a short-lived bearer token\n    (tokens expire hourly).\n  sources:\n  - openapi/zayo-group-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo-group/refs/heads/main/authentication/zayo-group-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fiber
- Network
- Infrastructure
---
