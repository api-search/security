---
api_key_in: []
api_specs:
- filename: sidequest-apps-api-openapi.yml
  format: yaml
  label: SideQuest Apps API
  slug: sidequest-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-apps-api-openapi.yml
- filename: sidequest-developers-api-openapi.yml
  format: yaml
  label: SideQuest Developers API
  slug: sidequest-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-developers-api-openapi.yml
- filename: sidequest-oauth2-api-openapi.yml
  format: yaml
  label: SideQuest OAuth2 API
  slug: sidequest-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-oauth2-api-openapi.yml
- filename: sidequest-users-api-openapi.yml
  format: yaml
  label: SideQuest Users API
  slug: sidequest-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-users-api-openapi.yml
- filename: sidequest-usersapps-api-openapi.yml
  format: yaml
  label: SideQuest UsersApps API
  slug: sidequest-usersapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/openapi/sidequest-usersapps-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sidequest Authentication
name_suffix: Authentication
oauth_flows: []
overview: SideQuest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SideQuest
provider_slug: sidequest
scheme_count: 1
schemes:
- name: userAuth
  scheme: bearer
  sources:
  - openapi/sidequest-openapi.json
  type: http
slug: sidequest-authentication
source_filename: sidequest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sidequest-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: userAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/sidequest-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidequest/refs/heads/main/authentication/sidequest-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- Virtual Reality
- VR
- XR
- Gaming
- App Store
- Developers
---
