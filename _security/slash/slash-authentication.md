---
api_key_in:
- header
api_specs:
- filename: slash-openapi-original.json
  format: json
  label: Slash Public API
  slug: slash-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/openapi/slash-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Slash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slash secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Slash
provider_slug: slash
scheme_count: 3
schemes:
- description: "API key authentication for public API requests.\n\nKeys come in two flavors:\n\n- *Legal-entity-scoped keys* are pinned to a single legal entity.\n  Minted via the dashboard under a specific entity; every request\n  acts on that entity.\n- *User-scoped keys* are pinned to a user and span every legal\n  entity that user has access to. Every request made with a\n  user-scoped key (except `GET /legal-entity`,"
  in: header
  name: api_key
  parameter: X-API-Key
  sources:
  - openapi/slash-openapi-original.json
  type: apiKey
- name: bearer
  scheme: bearer
  sources:
  - openapi/slash-openapi-original.json
  type: http
- name: developer_application
  scheme: basic
  sources:
  - openapi/slash-openapi-original.json
  type: http
slug: slash-authentication
source_filename: slash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/slash-openapi-original.json\ndocs: https://docs.slash.com/introduction\ntenancy_header:\n  name: x-legal-entity\n  required_for: user-scoped keys (except GET /legal-entity)\noauth_oidc:\n  note: >-\n    Third-party developer applications additionally use OAuth2/OIDC\n    (authorization_code, client_secret_basic) with the permission-key model in\n    scopes/slash-scopes.yml. Discovery at api.slash.com/.well-known/openid-configuration.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key authentication for public API requests.\n\n    Keys come in two flavors:\n\n    - *Legal-entity-scoped keys* are pinned to a single legal entity.\n      Minted via the dashboard under a specific entity; every request\n      acts on that entity.\n    - *User-scoped keys* are pinned to a user and span every legal\n\
  \      entity that user has access to. Every request made with a\n      user-scoped key (except `GET /legal-entity`,\n  sources:\n  - openapi/slash-openapi-original.json\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/slash-openapi-original.json\n- name: developer_application\n  type: http\n  scheme: basic\n  sources:\n  - openapi/slash-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/authentication/slash-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Banking
- Payments
- Financial Services
- Fintech
- Corporate Cards
- Business Banking
- Invoicing
- Expense Management
- Treasury
- FDX
---
