---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-gmail-domains-api-openapi.yml
  format: yaml
  label: Google Gmail Domains API
  slug: google-gmail-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-domains-api-openapi.yml
- filename: google-gmail-domainstats-api-openapi.yml
  format: yaml
  label: Google Gmail Domain Stats API
  slug: google-gmail-domainstats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-domainstats-api-openapi.yml
- filename: google-gmail-users-api-openapi.yml
  format: yaml
  label: Google Gmail Users API
  slug: google-gmail-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gmail/openapi/google-gmail-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Gmail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Gmail secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Gmail
provider_slug: google-gmail
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-gmail-gmail-users-api-openapi.yml
  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml
  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 26
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-gmail-gmail-users-api-openapi.yml
  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml
  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml
  type: oauth2
slug: google-gmail-authentication
source_filename: google-gmail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-gmail-gmail-users-api-openapi.yml, openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml,\n  openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 26\n  sources:\n  - openapi/google-gmail-gmail-users-api-openapi.yml\n  - openapi/google-gmail-gmailpostmastertools-domain-stats-api-openapi.yml\n\
  \  - openapi/google-gmail-gmailpostmastertools-domains-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-gmail/authentication/google-gmail-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Drafts
- Email
- Gmail
- Google
- Google Workspace
- Labels
- Messaging
- Threads
---
