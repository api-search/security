---
api_key_in: []
api_specs:
- filename: mindmaze-content-openapi.yml
  format: yaml
  label: MindMaze Therapeutics Content API
  slug: mindmaze-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-content-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mindmaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: MindMaze secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MindMaze
provider_slug: mindmaze
scheme_count: 2
schemes:
- applies_to: every operation in openapi/mindmaze-content-openapi.yml
  detail: All 17 captured operations return HTTP 200 with no credential. Verified live on 2026-08-01 against https://mindmazetherapeutics.com/wp-json.
  name: anonymous
  sources:
  - openapi/mindmaze-content-openapi.yml
  type: none
- applies_to: write and administrative routes, excluded from the captured OpenAPI
  authorization_endpoint: https://mindmazetherapeutics.com/wp-admin/authorize-application.php
  detail: The API index advertises WordPress Application Passwords as the only authentication method on the host. Credentials are issued from wp-admin to existing WordPress users - there is no self-serve sign-up, no developer account and no API key programme. Routes behind it (settings, themes, plugins, menus, block-types, widgets, all write methods) return {"code":"rest_forbidden","data":{"status":401}} anonymously.
  name: application-passwords
  scheme: basic
  self_serve: false
  sources:
  - https://mindmazetherapeutics.com/wp-json/
  type: http
slug: mindmaze-authentication
source_filename: mindmaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/mindmaze-content-openapi.yml + the live API index at https://mindmazetherapeutics.com/wp-json/\nnote: >-\n  derive-authentication.py produced no profile for this provider because the captured OpenAPI\n  declares no securitySchemes - correctly, since every captured operation is anonymous. This\n  file is written by hand from the same evidence so the auth model is recorded rather than\n  silently absent.\nsummary:\n  types: [none, http]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  developer_credential_available: false\nschemes:\n- name: anonymous\n  type: none\n  applies_to: every operation in openapi/mindmaze-content-openapi.yml\n  detail: >-\n    All 17 captured operations return HTTP 200 with no credential. Verified live on 2026-08-01\n    against https://mindmazetherapeutics.com/wp-json.\n  sources: [openapi/mindmaze-content-openapi.yml]\n- name: application-passwords\n  type: http\n  scheme: basic\n\
  \  applies_to: write and administrative routes, excluded from the captured OpenAPI\n  authorization_endpoint: https://mindmazetherapeutics.com/wp-admin/authorize-application.php\n  detail: >-\n    The API index advertises WordPress Application Passwords as the only authentication method\n    on the host. Credentials are issued from wp-admin to existing WordPress users - there is no\n    self-serve sign-up, no developer account and no API key programme. Routes behind it\n    (settings, themes, plugins, menus, block-types, widgets, all write methods) return\n    {\"code\":\"rest_forbidden\",\"data\":{\"status\":401}} anonymously.\n  sources: [https://mindmazetherapeutics.com/wp-json/]\n  self_serve: false\noauth:\n  present: false\n  detail: >-\n    No OAuth 2.0 or OpenID Connect surface. /.well-known/oauth-authorization-server,\n    /.well-known/oauth-protected-resource and /.well-known/openid-configuration all return 404\n    on every MindMaze host. No scopes/ artifact is written - there\
  \ is no scope surface to record.\ndocs: null\ndocs_note: >-\n  MindMaze publishes no authentication documentation, because it publishes no developer\n  programme. Everything above is observed behaviour, not a documented contract, and MindMaze\n  makes no commitment to keep it stable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/authentication/mindmaze-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Digital Therapeutics
- Neurotechnology
- Neurorehabilitation
- Medical Devices
- Health
- Artificial Intelligence
- Stroke
- Parkinsons Disease
- Switzerland
---
