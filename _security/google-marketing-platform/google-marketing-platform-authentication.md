---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Marketing Platform Admin API
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/openapi/openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Marketing Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Marketing Platform Admin secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-marketing-platform-authentication
source_filename: google-marketing-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/authentication/google-marketing-platform-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
---
