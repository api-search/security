---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Scnd Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
- authorizationCode
overview: Second (scnd) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, password, and authorizationCode flow(s).
provider_name: Second (scnd)
provider_slug: scnd
scheme_count: 1
schemes:
- flows:
  - description: Machine-to-machine authentication (client app is a server). Accesses Second API endpoints that do not require user permissions. The app exchanges its Client ID and Secret for a token used on all API requests.
    flow: clientCredentials
  - description: Resource Owner Password Credentials grant for trusted first-party client apps (e.g. a Second native mobile app that also collects the user's username/password at login).
    flow: password
  - description: User is redirected to the Second OAuth provider to approve the requested permissions before the client app acts on their behalf; requires a configured homepage URL and authorization callback URL. Supports an optional "plain code challenge method" (PKCE, plain or encrypted).
    flow: authorizationCode
  name: OAuth2
  permissions:
  - description: Access to all frontend endpoints where user auth is required.
    name: private
  - description: Access to all backend endpoints where admin (super-admin) auth is required.
    name: admin
  source: https://features.scnd.com/v2.0/superadmin/oauth
  type: oauth2
slug: scnd-authentication
source_filename: scnd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://features.scnd.com/v2.0/superadmin/oauth\ndocs: https://features.scnd.com/v2.0/superadmin/oauth\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, password, authorizationCode]\n  pkce: true\n  permission_model: [private, admin]\n  note: >-\n    Second exposes an OAuth 2.0 provider. Super-administrators register\n    \"Authorized apps\" from the back office (SBO > OAuth > Authorized apps),\n    which generates a Client ID and Client Secret used as the app credentials.\n    Endpoint URLs are not published in the docs; the model is described narratively.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://features.scnd.com/v2.0/superadmin/oauth\n  flows:\n  - flow: clientCredentials\n    description: >-\n      Machine-to-machine authentication (client app is a server). Accesses\n      Second API endpoints that do not require user permissions. The app\n      exchanges its Client ID and Secret for\
  \ a token used on all API requests.\n  - flow: password\n    description: >-\n      Resource Owner Password Credentials grant for trusted first-party client\n      apps (e.g. a Second native mobile app that also collects the user's\n      username/password at login).\n  - flow: authorizationCode\n    description: >-\n      User is redirected to the Second OAuth provider to approve the requested\n      permissions before the client app acts on their behalf; requires a\n      configured homepage URL and authorization callback URL. Supports an\n      optional \"plain code challenge method\" (PKCE, plain or encrypted).\n  permissions:\n  - name: private\n    description: Access to all frontend endpoints where user auth is required.\n  - name: admin\n    description: Access to all backend endpoints where admin (super-admin) auth is required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scnd/refs/heads/main/authentication/scnd-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketplace
- Services
- Vendor Management
- Payments
- OAuth
- SaaS
- Procurement
---
