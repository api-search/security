---
api_key_in:
- header
api_specs:
- filename: unsplash-openapi.yml
  format: yaml
  label: Unsplash API
  slug: unsplash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/openapi/unsplash-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Unsplash Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Unsplash secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Unsplash
provider_slug: unsplash
scheme_count: 2
schemes:
- description: 'Use `Authorization: Client-ID {YOUR_ACCESS_KEY}` for public API access. Alternatively pass as query param: `?client_id={YOUR_ACCESS_KEY}`'
  in: header
  name: ClientID
  parameter: Authorization
  sources:
  - openapi/unsplash-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://unsplash.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://unsplash.com/oauth/token
  name: OAuth2
  sources:
  - openapi/unsplash-openapi.yml
  type: oauth2
slug: unsplash-authentication
source_filename: unsplash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unsplash-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ClientID\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Use `Authorization: Client-ID {YOUR_ACCESS_KEY}` for public API access. Alternatively\n    pass as query param: `?client_id={YOUR_ACCESS_KEY}`'\n  sources:\n  - openapi/unsplash-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://unsplash.com/oauth/authorize\n    tokenUrl: https://unsplash.com/oauth/token\n    scopes: 8\n  sources:\n  - openapi/unsplash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/authentication/unsplash-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Photos
- Images
- Photography
- Stock Photos
- Creative
- Open Source
- Media
---
