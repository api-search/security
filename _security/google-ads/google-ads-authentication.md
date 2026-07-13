---
api_key_in: []
api_specs:
- filename: google-ads-api-openapi.yml
  format: yaml
  label: Google Ads API
  slug: google-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Ads secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Ads
provider_slug: google-ads
scheme_count: 1
schemes:
- description: 'Google Ads API uses OAuth 2.0 for authentication. Requires a developer

    token, OAuth 2.0 client ID and secret, and a refresh token.'
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2Auth
  sources:
  - openapi/google-ads-api-openapi.yml
  type: oauth2
slug: google-ads-authentication
source_filename: google-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-ads-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: |-\n    Google Ads API uses OAuth 2.0 for authentication. Requires a developer\n    token, OAuth 2.0 client ID and secret, and a refresh token.\n  sources:\n  - openapi/google-ads-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/authentication/google-ads-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Campaign Management
- Digital Advertising
- Google
- Marketing
- PPC
---
