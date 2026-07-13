---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google People API
  slug: google-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-people/refs/heads/main/openapi/openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google People Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google People secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google People
provider_slug: google-people
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-people-authentication
source_filename: google-people-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-people/refs/heads/main/authentication/google-people-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Address Book
- Contacts
- Google
- People
- Profiles
---
