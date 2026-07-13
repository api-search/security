---
api_key_in: []
api_specs:
- filename: wildapricot-admin-api-openapi.yml
  format: yaml
  label: WildApricot Admin API
  slug: wildapricot-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/openapi/wildapricot-admin-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wildapricot Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: WildApricot secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: WildApricot
provider_slug: wildapricot
scheme_count: 1
schemes:
- description: OAuth2 authentication for WildApricot API
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://oauth.wildapricot.org/auth/token
  name: OAuth2
  sources:
  - openapi/wildapricot-admin-api-openapi.yml
  type: oauth2
slug: wildapricot-authentication
source_filename: wildapricot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wildapricot-admin-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.wildapricot.org/auth/token\n    scopes: 1\n  description: OAuth2 authentication for WildApricot API\n  sources:\n  - openapi/wildapricot-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/authentication/wildapricot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Membership Management
- Associations
- Nonprofit
- Events
- Payments
---
