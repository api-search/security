---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-looker-studio-assets-search-api-openapi.yml
  format: yaml
  label: Google Looker Studio Assets:search API
  slug: google-looker-studio-assets-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/openapi/google-looker-studio-assets-search-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Looker Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Looker Studio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Looker Studio
provider_slug: google-looker-studio
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-looker-studio-assets-search-api-openapi.yml
  - https://developers.google.com/looker-studio/api
  type: oauth2
slug: google-looker-studio-authentication
source_filename: google-looker-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: openapi/google-looker-studio-assets-search-api-openapi.yml\ndocs: https://developers.google.com/looker-studio/api\nevidence:\n- url: https://developers.google.com/looker-studio/api\n  status: 200\n  kind: provider authentication + authorization guide\n- url: https://datastudio.googleapis.com/v1/assets:search?assetTypes=REPORT\n  status: 401\n  kind: live probe — WWW-Authenticate challenge observed\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_keys: false\n  mtls: false\n  challenge: 'WWW-Authenticate: Bearer realm=\"https://accounts.google.com/\"'\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/google-looker-studio-assets-search-api-openapi.yml\n  - https://developers.google.com/looker-studio/api\npreconditions:\n\
  - id: workspace-membership\n  requirement: >-\n    The authenticating user must belong to a Google Workspace or Cloud Identity organization.\n    Consumer Google accounts cannot authenticate to this API at all.\n- id: domain-wide-delegation\n  requirement: >-\n    A Workspace admin must register the app's OAuth client ID under domain-wide delegation in the\n    Google Admin console, together with the scopes the app needs, before any user in that\n    organization can authorize the app. Once done, every user in the organization is authorized\n    automatically and is shown no OAuth consent dialog.\n  admin_surface: https://admin.google.com/ac/owl/domainwidedelegation\n- id: api-enabled\n  requirement: The Data Studio API must be enabled on the caller's Google Cloud project.\n- id: do-not-self-declare-scopes\n  requirement: >-\n    Google instructs developers NOT to add Data Studio scopes to their own OAuth client; the\n    Workspace admin attaches them during delegation. Declaring them\
  \ locally is the documented cause\n    of the Error 400 invalid_scope failure.\nfailure_modes:\n- error: 'Error 400: invalid_scope'\n  cause: The user's organization has not authorized the app, or authorized it with the wrong scopes.\n  remedy: The user must ask their Workspace admin to complete or correct the delegation.\n- error: 401 UNAUTHENTICATED / CREDENTIALS_MISSING\n  cause: No or expired bearer token.\n- error: 403 PERMISSION_DENIED\n  cause: API not enabled on the project, or caller has no established identity.\ncross_links:\n  scopes: scopes/google-looker-studio-scopes.yml\n  conventions: conventions/google-looker-studio-conventions.yml\n  errors: errors/google-looker-studio-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/authentication/google-looker-studio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
---
