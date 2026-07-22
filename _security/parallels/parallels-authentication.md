---
api_key_in:
- header
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Parallels Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallels secures its APIs with token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parallels
provider_slug: parallels
scheme_count: 2
schemes:
- description: Log on with administrator credentials to obtain an authToken, then send it in the auth_token header on all subsequent requests. Tokens are session-scoped.
  in: header
  logon_body: '{"username": "...", "password": "...", "tenantId": ...}'
  logon_endpoint: POST https://<API-host>:20443/api/session/logon
  name: RASAuthToken
  parameter: auth_token
  response_field: authToken
  type: token
- description: Parallels Desktop Enterprise and the Management Portal support SSO with Azure/Entra ID, Okta, Ping Identity, JumpCloud, and Google Workspace via Parallels My Account (product sign-in, distinct from the RAS REST API token).
  name: SSO
  scope: Parallels My Account / Management Portal
  type: sso
slug: parallels-authentication
source_filename: parallels-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.parallels.com/landing/ras-rest-api-guide\ndocs: https://docs.parallels.com/landing/ras-rest-api-guide\nnotes: >-\n  The Parallels RAS REST API is a self-hosted admin API (no downloadable OpenAPI\n  spec is published). Authentication is a bespoke token scheme: administrators POST\n  credentials to a logon endpoint and receive an authToken that is echoed on every\n  subsequent request via the auth_token header. Not OAuth2/OIDC.\nsummary:\n  types: [token]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: RASAuthToken\n  type: token\n  in: header\n  parameter: auth_token\n  logon_endpoint: 'POST https://<API-host>:20443/api/session/logon'\n  logon_body: '{\"username\": \"...\", \"password\": \"...\", \"tenantId\": ...}'\n  response_field: authToken\n  description: >-\n    Log on with administrator credentials to obtain an authToken, then send it in\n    the auth_token header on all subsequent requests.\
  \ Tokens are session-scoped.\n- name: SSO\n  type: sso\n  scope: Parallels My Account / Management Portal\n  description: >-\n    Parallels Desktop Enterprise and the Management Portal support SSO with\n    Azure/Entra ID, Okta, Ping Identity, JumpCloud, and Google Workspace via\n    Parallels My Account (product sign-in, distinct from the RAS REST API token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallels/refs/heads/main/authentication/parallels-authentication.yml
summary_line: token · 2 schemes
tags:
- Company
- Virtualization
- Remote Desktop
- VDI
- DaaS
- Mac
- Infrastructure
- IT Management
---
