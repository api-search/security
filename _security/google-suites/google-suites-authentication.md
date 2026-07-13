---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Gmail API
  slug: gmail-api
  spec_type: OpenAPI
  url: https://gmail.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Calendar API
  slug: google-calendar-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/calendar/v3/rest
- filename: rest
  format: yaml
  label: Google Drive API
  slug: google-drive-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/drive/v3/rest
- filename: rest
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://docs.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://sheets.googleapis.com/$discovery/rest?version=v4
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Admin SDK Directory API
  slug: admin-sdk-directory-api
  spec_type: OpenAPI
  url: https://admin.googleapis.com/$discovery/rest?version=directory_v1
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Suites Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Workspace APIs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Workspace APIs
provider_slug: google-suites
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  sources:
  - openapi/google-suites-openapi.yml
  type: oauth2
slug: google-suites-authentication
source_filename: google-suites-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suites-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: googleOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 6\n  sources:\n  - openapi/google-suites-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suites/refs/heads/main/authentication/google-suites-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud Storage
- Collaboration
- Email
- Office Suite
- Productivity
---
