---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cutover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cutover secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cutover
provider_slug: cutover
scheme_count: 1
schemes:
- bearerFormat: opaque-48-char-token
  description: Authentication is performed via bearer authentication using a User App Token, a 48-character (192-bit) opaque string. Tokens are created in the Cutover application under Access Management for a non-interactive user that holds the Developer role plus any additional roles required for the calls it makes. The token is displayed only once at creation and can be revoked or set to expire by a Global User Admin.
  format: 'Authorization: Bearer <user_app_token>'
  header: Authorization
  location: header
  name: userAppToken
  scheme: bearer
  type: http
slug: cutover-authentication
source_filename: cutover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.cutover.com/cutover-api/authentication\ndocs: https://developer.cutover.com/cutover-api/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  model: role-based access control (no OAuth scopes)\nschemes:\n- name: userAppToken\n  type: http\n  scheme: bearer\n  bearerFormat: opaque-48-char-token\n  location: header\n  header: Authorization\n  format: 'Authorization: Bearer <user_app_token>'\n  description: >-\n    Authentication is performed via bearer authentication using a User App Token,\n    a 48-character (192-bit) opaque string. Tokens are created in the Cutover\n    application under Access Management for a non-interactive user that holds the\n    Developer role plus any additional roles required for the calls it makes.\n    The token is displayed only once at creation and can be revoked or set to\n    expire by a Global User Admin.\nauthorization:\n\
  \  model: rbac\n  notes: >-\n    There is no OAuth or scopes system. Access is governed by role-based access\n    control: the non-interactive user behind a token must hold the Developer role\n    plus the specific additional roles (e.g. Workspace Manager, Integrations Admin,\n    Global User Admin) needed for the resources it touches. A 403 Forbidden is\n    returned when the token's roles are insufficient.\ntoken_management:\n  created_in: Access Management > User > User App Tokens\n  display: shown once at creation\n  expiry: configurable (arranged via Customer Success Manager)\n  revocation: Global User Admin can revoke tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutover/refs/heads/main/authentication/cutover-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Business Applications
- IT Operations
- Disaster Recovery
- Incident Management
- Runbook Automation
- Orchestration
- Workflow Automation
- DevOps
---
