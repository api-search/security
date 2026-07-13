---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Slides Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Slides secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Slides
provider_slug: google-slides
scheme_count: 1
schemes:
- description: Google OAuth 2.0 authentication. Requires one of the following scopes depending on the operation.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-slides-api-openapi.yml
  type: oauth2
slug: google-slides-authentication
source_filename: google-slides-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-slides-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 7\n  description: Google OAuth 2.0 authentication. Requires one of the following scopes depending\n    on the operation.\n  sources:\n  - openapi/google-slides-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/authentication/google-slides-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
---
