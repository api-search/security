---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nest Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nest secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nest
provider_slug: nest
scheme_count: 1
schemes:
- authorizationUrl: https://nestservices.google.com/partnerconnections/{project-id}/auth
  flow: authorizationCode
  name: GoogleOAuth2
  notes: 'Authorization uses Google''s Partner Connections Manager URL (scoped to the Device Access project id) rather than the generic accounts.google.com consent screen. Access tokens are Google OAuth bearer tokens presented as `Authorization: Bearer <token>` against https://smartdevicemanagement.googleapis.com.'
  scopes:
  - description: Access, control and manage the user's authorized Nest devices via the SDM API
    scope: https://www.googleapis.com/auth/sdm.service
  sources:
  - https://developers.google.com/nest/device-access/authorize
  tokenUrl: https://www.googleapis.com/token
  type: oauth2
slug: nest-authentication
source_filename: nest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.google.com/nest/device-access/authorize\ndocs: https://developers.google.com/nest/device-access/authorize\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Nest Smart Device Management (SDM) API is a Google Cloud API and is\n    authorized exclusively with Google OAuth 2.0 (authorization code flow).\n    A Device Access project (created in the Device Access Console) plus a\n    Google Cloud OAuth 2.0 client ID are required. End users grant access to\n    their Nest devices through the Partner Connections Manager consent screen.\nschemes:\n  - name: GoogleOAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://nestservices.google.com/partnerconnections/{project-id}/auth\n    tokenUrl: https://www.googleapis.com/token\n    scopes:\n      - scope: https://www.googleapis.com/auth/sdm.service\n        description: Access, control and manage the\
  \ user's authorized Nest devices via the SDM API\n    sources: [https://developers.google.com/nest/device-access/authorize]\n    notes: >-\n      Authorization uses Google's Partner Connections Manager URL (scoped to the\n      Device Access project id) rather than the generic accounts.google.com\n      consent screen. Access tokens are Google OAuth bearer tokens presented as\n      `Authorization: Bearer <token>` against https://smartdevicemanagement.googleapis.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nest/refs/heads/main/authentication/nest-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Hardware
- Smart Home
- IoT
- Home Automation
- Thermostat
- Google
- Device Access
---
