---
api_key_in:
- header
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Places API
  slug: google-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Places Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Places secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Places
provider_slug: google-places
scheme_count: 3
schemes:
- description: Google Maps Platform API key passed in the X-Goog-Api-Key header.
  in: header
  name: ApiKeyAuth
  parameter: X-Goog-Api-Key
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: Google Maps Platform API key passed as the key query parameter.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: OAuth 2.0 bearer token authorization for the Google Maps Platform.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/openapi.yml
  type: oauth2
slug: google-places-authentication
source_filename: google-places-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Goog-Api-Key\n  description: Google Maps Platform API key passed in the X-Goog-Api-Key header.\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Google Maps Platform API key passed as the key query parameter.\n  sources:\n  - openapi/openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: OAuth 2.0 bearer token authorization for the Google Maps Platform.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/authentication/google-places-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Restaurant
- Geolocation
- Google
- Locations
- Maps
- Places
- Points of Interest
---
