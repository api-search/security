---
api_key_in: []
api_specs:
- filename: google-docs-api-v1-openapi.yml
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/openapi/google-docs-api-v1-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Docs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Docs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Docs
provider_slug: google-docs
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for Google APIs.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-docs-api-v1-openapi.yml
  type: oauth2
slug: google-docs-authentication
source_filename: google-docs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-docs-api-v1-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 5\n  description: OAuth 2.0 authentication for Google APIs.\n  sources:\n  - openapi/google-docs-api-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/authentication/google-docs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
---
