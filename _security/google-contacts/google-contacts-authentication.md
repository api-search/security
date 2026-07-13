---
api_key_in: []
api_specs:
- filename: contacts.yml
  format: yaml
  label: Google People API v1
  slug: google-people-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/openapi/contacts.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Contacts Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google People API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google People API
provider_slug: google-contacts
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/contacts.yml
  type: oauth2
slug: google-contacts-authentication
source_filename: google-contacts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contacts.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 4\n  sources:\n  - openapi/contacts.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/authentication/google-contacts-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Address Book
- Contacts
- Directory
- Google
- People
- Profiles
---
