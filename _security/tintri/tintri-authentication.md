---
api_key_in: []
auth_types:
- session
description: The Tintri VMstore REST API (v310) uses session-based authentication. A client authenticates with local or directory-service credentials by POSTing to the session/login endpoint; the server returns a session cookie (JSESSIONID) that must accompany subsequent requests. There is no OAuth 2.0 / OpenID Connect flow and no long-lived API-key surface — sessions are short-lived and are explicitly closed via session/logout. Because there is no OAuth scope model, no scopes/ artifact is produced; role-based access control is enforced by the appliance against the authenticated user's assigned UserRole.
kind: authentication
layout: security
method: searched
name: Tintri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tintri secures its APIs with session across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tintri
provider_slug: tintri
scheme_count: 1
schemes:
- authorization_model: role-based access control (UserRole) enforced by the appliance
  cookie_name: JSESSIONID
  login: POST /api/v310/session/login
  login_body: '{ "username": "...", "password": "...", "typeId": "com.tintri.api.rest.vcommon.dto.rbac.RestApiCredentials" }'
  logout: GET /api/v310/session/logout
  name: sessionAuth
  scheme: cookie
  sources:
  - docs
  type: session
slug: tintri-authentication
source_filename: tintri-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tintri.github.io/tintri-rest-api/index.html\ndocs: https://tintri.github.io/tintri-rest-api/index.html\ndescription: >-\n  The Tintri VMstore REST API (v310) uses session-based authentication. A client\n  authenticates with local or directory-service credentials by POSTing to the\n  session/login endpoint; the server returns a session cookie (JSESSIONID) that\n  must accompany subsequent requests. There is no OAuth 2.0 / OpenID Connect\n  flow and no long-lived API-key surface — sessions are short-lived and are\n  explicitly closed via session/logout. Because there is no OAuth scope model,\n  no scopes/ artifact is produced; role-based access control is enforced by the\n  appliance against the authenticated user's assigned UserRole.\nsummary:\n  types: [session]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: sessionAuth\n  type: session\n  scheme: cookie\n  cookie_name: JSESSIONID\n  login: POST /api/v310/session/login\n\
  \  login_body: '{ \"username\": \"...\", \"password\": \"...\", \"typeId\": \"com.tintri.api.rest.vcommon.dto.rbac.RestApiCredentials\" }'\n  logout: GET /api/v310/session/logout\n  authorization_model: role-based access control (UserRole) enforced by the appliance\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tintri/refs/heads/main/authentication/tintri-authentication.yml
summary_line: session · 1 scheme
tags:
- Company
- Storage
- Data Management
- Infrastructure
- Virtualization
- Cloud
- Kubernetes
- DevOps
- Enterprise
- REST API
---
