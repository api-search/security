---
api_key_in: []
api_specs:
- filename: google-tag-manager-api-v2-openapi.yml
  format: yaml
  label: Google Tag Manager API
  slug: google-tag-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-api-v2-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Tag Manager Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Tag Manager secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Tag Manager
provider_slug: google-tag-manager
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication for Google Tag Manager API.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-tag-manager-api-v2-openapi.yml
  type: oauth2
slug: google-tag-manager-authentication
source_filename: google-tag-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-tag-manager-api-v2-openapi.yml\ndocs: https://developers.google.com/tag-platform/tag-manager/api/v2/authorization\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 7\n  description: OAuth 2.0 authentication for Google Tag Manager API.\n  sources:\n  - openapi/google-tag-manager-api-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/authentication/google-tag-manager-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
---
