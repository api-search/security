---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-keep-notes-api-openapi.yml
  format: yaml
  label: Google Keep Notes API
  slug: google-keep-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-keep/openapi/google-keep-notes-api-openapi.yml
- filename: google-keep-media-api-openapi.yml
  format: yaml
  label: Google Keep Keep Media API
  slug: google-keep-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-keep/openapi/google-keep-media-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Google Keep Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Keep secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Keep
provider_slug: google-keep
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-keep-media-api-openapi.yml
  - openapi/google-keep-notes-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-keep-media-api-openapi.yml
  - openapi/google-keep-notes-api-openapi.yml
  type: oauth2
slug: google-keep-authentication
source_filename: google-keep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://developers.google.com/workspace/keep/api/guides/java\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-keep-media-api-openapi.yml\n  - openapi/google-keep-notes-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-keep-media-api-openapi.yml\n  - openapi/google-keep-notes-api-openapi.yml\ndocs: https://developers.google.com/workspace/keep/api/guides/java\nnote: Docs require a service account with domain-wide delegation granted by a Workspace\n  super administrator to call on behalf of users.\n"
source_yaml_url: https://artifacts.apis.io/google-keep/authentication/google-keep-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Google
- Google Workspace
- Notes
- Organization
- Productivity
---
