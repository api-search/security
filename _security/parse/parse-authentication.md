---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Parse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parse secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parse
provider_slug: parse
scheme_count: 5
schemes:
- description: Identifies which Parse application the request targets. Required on every REST request.
  in: header
  name: X-Parse-Application-Id
  required: true
  type: apiKey
- description: Client REST API key. Grants client-level access subject to class-level permissions (CLP) and per-object ACLs.
  in: header
  name: X-Parse-REST-API-Key
  type: apiKey
- description: Master key. Full read/write access that bypasses all ACLs and CLPs. Use only from trusted server-side environments; never ship in client apps.
  in: header
  name: X-Parse-Master-Key
  type: apiKey
- description: Per-user session token returned by signup/login. Scopes a request to the permissions of that authenticated user.
  in: header
  name: X-Parse-Session-Token
  type: apiKey
- description: Set to "1" on login/signup to request a revocable session token stored in the _Session class (recommended over legacy tokens).
  in: header
  name: X-Parse-Revocable-Session
  type: apiKey
slug: parse-authentication
source_filename: parse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.parseplatform.org/rest/guide/\ndocs: https://docs.parseplatform.org/rest/guide/#getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: >-\n    Parse REST authentication is header-based. Every request identifies the\n    application with X-Parse-Application-Id and authorizes with a client key\n    (X-Parse-REST-API-Key), the Master Key (X-Parse-Master-Key, bypasses ACL/CLP),\n    or an end-user session token (X-Parse-Session-Token). There is no OAuth2/OIDC\n    surface at the Parse Server REST layer.\nschemes:\n  - name: X-Parse-Application-Id\n    type: apiKey\n    in: header\n    required: true\n    description: >-\n      Identifies which Parse application the request targets. Required on every\n      REST request.\n  - name: X-Parse-REST-API-Key\n    type: apiKey\n    in: header\n    description: >-\n      Client REST API key. Grants client-level access subject to class-level\n\
  \      permissions (CLP) and per-object ACLs.\n  - name: X-Parse-Master-Key\n    type: apiKey\n    in: header\n    description: >-\n      Master key. Full read/write access that bypasses all ACLs and CLPs. Use\n      only from trusted server-side environments; never ship in client apps.\n  - name: X-Parse-Session-Token\n    type: apiKey\n    in: header\n    description: >-\n      Per-user session token returned by signup/login. Scopes a request to the\n      permissions of that authenticated user.\n  - name: X-Parse-Revocable-Session\n    type: apiKey\n    in: header\n    description: >-\n      Set to \"1\" on login/signup to request a revocable session token stored in\n      the _Session class (recommended over legacy tokens).\nnotes:\n  - Master key and REST API key are configured on the Parse Server instance, not\n    minted per-request.\n  - Access control is enforced through per-object ACLs and per-class Class-Level\n    Permissions (CLP); the Master Key overrides both.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parse/refs/heads/main/authentication/parse-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Company
- Backend as a Service
- BaaS
- Mobile
- Open Source
- REST API
- Database
- Authentication
- Push Notifications
- Real Time
---
