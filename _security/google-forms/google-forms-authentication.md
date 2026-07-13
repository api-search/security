---
api_key_in: []
api_specs:
- filename: google-forms-api.yaml
  format: yaml
  label: Google Forms API v1
  slug: google-forms-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/openapi/google-forms-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Forms Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Forms secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Forms
provider_slug: google-forms
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for Google Forms API.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-forms-api.yaml
  type: oauth2
slug: google-forms-authentication
source_filename: google-forms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-forms-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 6\n  description: OAuth 2.0 authentication for Google Forms API.\n  sources:\n  - openapi/google-forms-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/authentication/google-forms-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
---
