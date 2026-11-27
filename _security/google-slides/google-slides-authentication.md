---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-slides-presentations-api-openapi.yml
  format: yaml
  label: Google Slides Presentations API
  slug: google-slides-presentations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-slides/openapi/google-slides-presentations-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
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
  - openapi/google-slides-presentations-api-openapi.yml
  - https://developers.google.com/workspace/slides/api/guides/authorizing
  type: oauth2
slug: google-slides-authentication
source_filename: google-slides-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://developers.google.com/workspace/slides/api/guides/authorizing\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  sources:\n  - openapi/google-slides-presentations-api-openapi.yml\n  - openapi/_superseded/google-slides-pages-api-openapi.yml\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 7\n  description: Google OAuth 2.0 authentication. Requires one of the following scopes\n    depending on the operation.\n  sources:\n  - openapi/google-slides-presentations-api-openapi.yml\n  - https://developers.google.com/workspace/slides/api/guides/authorizing\ndocs: https://developers.google.com/workspace/guides/auth-overview\n"
source_yaml_url: https://artifacts.apis.io/google-slides/authentication/google-slides-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
---
