---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-chrome-challenge-api-openapi.yml
  format: yaml
  label: Google Chrome Challenge API
  slug: google-chrome-challenge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-challenge-api-openapi.yml
- filename: google-chrome-customers-api-openapi.yml
  format: yaml
  label: Google Chrome Customers API
  slug: google-chrome-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-customers-api-openapi.yml
- filename: google-chrome-media-api-openapi.yml
  format: yaml
  label: Google Chrome Media API
  slug: google-chrome-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-media-api-openapi.yml
- filename: google-chrome-operations-api-openapi.yml
  format: yaml
  label: Google Chrome Operations API
  slug: google-chrome-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-operations-api-openapi.yml
- filename: google-chrome-platforms-api-openapi.yml
  format: yaml
  label: Google Chrome Platforms API
  slug: google-chrome-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-platforms-api-openapi.yml
- filename: google-chrome-publishers-api-openapi.yml
  format: yaml
  label: Google Chrome Publishers API
  slug: google-chrome-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-publishers-api-openapi.yml
- filename: google-chrome-records-api-openapi.yml
  format: yaml
  label: Google Chrome Records API
  slug: google-chrome-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chrome/openapi/google-chrome-records-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Chrome Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Chrome secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Chrome
provider_slug: google-chrome
scheme_count: 1
schemes:
- description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-chrome-management-api-openapi.json
  type: oauth2
slug: google-chrome-authentication
source_filename: google-chrome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-chrome-management-api-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.\n  sources:\n  - openapi/google-chrome-management-api-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/google-chrome/authentication/google-chrome-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Browser
- Chrome Extensions
- Developer Tools
- Web Platform
---
