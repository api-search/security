---
api_key_in: []
api_specs:
- filename: google-display-video-360-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 API
  slug: google-display-video-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-api-openapi.yml
- filename: google-display-video-360-advertisers-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 Advertisers API
  slug: google-display-video-360-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-advertisers-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Display Video 360 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Display & Video 360 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Display & Video 360
provider_slug: google-display-video-360
scheme_count: 1
schemes:
- description: Google OAuth 2.0. Authorization and token endpoints read from https://accounts.google.com/.well-known/openid-configuration.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-display-video-360-advertisers-api-openapi.yml
  - openapi/google-display-video-360-api-openapi.yml
  type: oauth2
slug: google-display-video-360-authentication
source_filename: google-display-video-360-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/google-display-video-360-advertisers-api-openapi.yml, openapi/google-display-video-360-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 4\n  description: Google OAuth 2.0. Authorization and token endpoints read from https://accounts.google.com/.well-known/openid-configuration.\n  sources:\n  - openapi/google-display-video-360-advertisers-api-openapi.yml\n  - openapi/google-display-video-360-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/authentication/google-display-video-360-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Campaign Management
- Display Ads
- DV360
- Programmatic Advertising
- Targeting
- Video Ads
- Advertising
- AdTech
- Demand-Side Platform
- Media Buying
- Audiences
- Google Marketing Platform
---
