---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Business Profile API
  slug: google-business-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-business-profile/refs/heads/main/openapi/openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Business Profile Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Business Profile secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Business Profile
provider_slug: google-business-profile
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-business-profile-authentication
source_filename: google-business-profile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-business-profile/refs/heads/main/authentication/google-business-profile-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Profiles
- Google
- Local Business
- Locations
- Reviews
---
