---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cask Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cask Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cask Data
provider_slug: cask-data
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <cdap-access-token>'
  header: Authorization
  in: header
  mechanisms_supported:
  - basic
  - ldap
  - jaspi
  - custom
  name: bearerToken
  obtained_via:
  - library: io.cdap.cdap:cdap-authentication-client
  - endpoint: GET /v3/security/... (authentication server)
  scheme: bearer
  sources:
  - docs
  type: http
slug: cask-data-authentication
source_filename: cask-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cdap.io/cdap/current/en/admin-manual/security/index.html\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  CDAP supports optional perimeter security. When security is enabled, clients first obtain an\n  access token from the CDAP authentication server (via the cdap-authentication-client library or\n  the /v3/security endpoints) using a configured authentication mechanism (basic, LDAP, JASPI, or\n  a custom handler), then present it as a Bearer token on every HTTP RESTful API request. On an\n  unsecured (default sandbox) deployment no credentials are required. There is no OAuth 2.0 scope\n  surface, so no scopes/ artifact is produced.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Authorization: Bearer <cdap-access-token>\"\n  obtained_via:\n  - library: io.cdap.cdap:cdap-authentication-client\n\
  \  - endpoint: GET /v3/security/... (authentication server)\n  mechanisms_supported: [basic, ldap, jaspi, custom]\n  sources: [docs]\nunsecured_default:\n  note: The CDAP Sandbox runs with security disabled by default; requests to /v3/namespaces require no token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cask-data/refs/heads/main/authentication/cask-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Data Integration
- Data Pipelines
- ETL
- Big Data
- Analytics
- Open Source
- Hadoop
- CDAP
---
