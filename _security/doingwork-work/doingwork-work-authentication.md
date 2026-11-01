---
anonymous_access: false
api_key_in: []
api_specs:
- filename: doingwork-work-status-api-openapi.yml
  format: yaml
  label: doingwork-work Status API
  slug: doingwork-work-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doingwork-work/openapi/doingwork-work-status-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Doingwork Work Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: doingwork-work secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: doingwork-work
provider_slug: doingwork-work
scheme_count: 1
schemes:
- description: 'Authorization code flow with PKCE (S256). Dynamic client registration at /oauth/register. Metadata: https://app.doingwork.work/.well-known/oauth-authorization-server'
  flows:
  - authorizationUrl: https://app.doingwork.work/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://app.doingwork.work/oauth/token
  name: doingWorkOAuth
  sources:
  - openapi/doingwork-work-openapi.json
  type: oauth2
slug: doingwork-work-authentication
source_filename: doingwork-work-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/doingwork-work-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: doingWorkOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.doingwork.work/oauth/authorize\n    tokenUrl: https://app.doingwork.work/oauth/token\n    scopes: 4\n  description: 'Authorization code flow with PKCE (S256). Dynamic client registration at /oauth/register.\n    Metadata: https://app.doingwork.work/.well-known/oauth-authorization-server'\n  sources:\n  - openapi/doingwork-work-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/doingwork-work/authentication/doingwork-work-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Field Service
- Invoicing
- API
- Mobile
---
