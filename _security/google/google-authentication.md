---
api_key_in:
- header
api_specs:
- filename: books-api-openapi.yml
  format: yaml
  label: Books API
  slug: books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/books-api-openapi.yml
- filename: google-drive-api-openapi.yml
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-api-openapi.yml
- filename: google-drive-activity-api-openapi.yml
  format: yaml
  label: Google Drive Activity API
  slug: google-drive-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-activity-api-openapi.yml
- filename: google-drive-labels-api-openapi.yml
  format: yaml
  label: Google Drive Labels API
  slug: google-drive-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-drive-labels-api-openapi.yml
- filename: google-calendar-api-openapi.yml
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-calendar-api-openapi.yml
- filename: google-gmail-api-openapi.yml
  format: yaml
  label: Google Gmail API
  slug: google-gmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gmail-api-openapi.yml
- filename: google-sheets-api-openapi.yml
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-sheets-api-openapi.yml
- filename: google-docs-api-openapi.yml
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-docs-api-openapi.yml
- filename: google-places-api-openapi.yml
  format: yaml
  label: Google Places API
  slug: google-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-places-api-openapi.yml
- filename: google-gemini-api-openapi.yml
  format: yaml
  label: Google Gemini API
  slug: google-gemini-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/openapi/google-gemini-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Google secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Google
provider_slug: google
scheme_count: 4
schemes:
- description: OAuth 2.0 authentication for Google Books API
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/books-api-openapi.yml
  - openapi/google-docs-api-openapi.yml
  - openapi/google-drive-activity-api-openapi.yml
  - openapi/google-drive-api-openapi.yml
  - openapi/google-drive-labels-api-openapi.yml
  type: oauth2
- name: oauth2Auth
  scheme: oauth2
  sources:
  - openapi/google-calendar-api-openapi.yml
  - openapi/google-gmail-api-openapi.yml
  - openapi/google-sheets-api-openapi.yml
  type: http
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
    scopes: 5
  name: Oauth2
  sources:
  - openapi/google-docs-api-openapi.yml
  - openapi/google-drive-activity-api-openapi.yml
  - openapi/google-drive-api-openapi.yml
  - openapi/google-drive-labels-api-openapi.yml
  type: oauth2
- description: API key for authentication
  in: header
  name: ApiKeyHeader
  parameter: x-goog-api-key
  sources:
  - openapi/google-gemini-api-openapi.yml
  type: apiKey
slug: google-authentication
source_filename: google-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/books-api-openapi.yml, openapi/google-calendar-api-openapi.yml, openapi/google-docs-api-openapi.yml,\n  openapi/google-drive-activity-api-openapi.yml, openapi/google-drive-api-openapi.yml, openapi/google-drive-labels-api-openapi.yml,\n  openapi/google-gemini-api-openapi.yml, openapi/google-gmail-api-openapi.yml, openapi/google-sheets-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: OAuth 2.0 authentication for Google Books API\n  sources:\n  - openapi/books-api-openapi.yml\n  - openapi/google-docs-api-openapi.yml\n  - openapi/google-drive-activity-api-openapi.yml\n  - openapi/google-drive-api-openapi.yml\n\
  \  - openapi/google-drive-labels-api-openapi.yml\n- name: oauth2Auth\n  type: http\n  scheme: oauth2\n  sources:\n  - openapi/google-calendar-api-openapi.yml\n  - openapi/google-gmail-api-openapi.yml\n  - openapi/google-sheets-api-openapi.yml\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    scopes: 5\n  description: Oauth 2.0 implicit authentication\n  sources:\n  - openapi/google-docs-api-openapi.yml\n  - openapi/google-drive-activity-api-openapi.yml\n  - openapi/google-drive-api-openapi.yml\n  - openapi/google-drive-labels-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-goog-api-key\n  description: API key for authentication\n  sources:\n  - openapi/google-gemini-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google/refs/heads/main/authentication/google-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Advertising
- Cloud
- Developer
- Google
- Platform
- Search
- T1
---
