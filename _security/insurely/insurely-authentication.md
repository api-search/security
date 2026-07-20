---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Insurely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insurely secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Insurely
provider_slug: insurely
scheme_count: 2
schemes:
- description: Static, tenant-level API key for backend operations (create/find/delete users, mint sessions, list a user's consents/collections by API-key auth). Obtained from Insurely support (support@insurely.com).
  in: header
  name: apiKeyAuth
  parameter_name: authorization-token
  sources:
  - docs.insurely.com
  type: apiKey
  used_for:
  - users
  - sessions
  - company availability
  - backend list operations
- bearer_format: JWT
  description: Per-user JWT session token for consumer-scoped operations (create/list consents, initiate/list collections, retrieve wealth data). Minted from the backend API key via the sessions endpoint and scoped to a single end user.
  in: header
  name: bearerAuth
  parameter_name: Authorization
  scheme: bearer
  sources:
  - docs.insurely.com
  type: http
  used_for:
  - consents
  - collections
  - wealth data
slug: insurely-authentication
source_filename: insurely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.insurely.com/integration/api/quick-start/\ndocs: https://docs.insurely.com/integration/api/collecting-psd2-data/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  notes: >-\n    Dual-credential model. Backend/server-to-server operations authenticate with\n    a static API key sent in the `authorization-token` header (issued by Insurely\n    via support@insurely.com). User-scoped operations (consents, collections)\n    authenticate with a short-lived per-user JWT session token minted via\n    POST /users/{userUuid}/sessions and sent as a standard Bearer token.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: authorization-token\n  description: >-\n    Static, tenant-level API key for backend operations (create/find/delete users,\n    mint sessions, list a user's consents/collections by API-key auth). Obtained\n    from Insurely support (support@insurely.com).\n\
  \  used_for: [users, sessions, company availability, backend list operations]\n  sources: [docs.insurely.com]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Per-user JWT session token for consumer-scoped operations (create/list consents,\n    initiate/list collections, retrieve wealth data). Minted from the backend API key\n    via the sessions endpoint and scoped to a single end user.\n  used_for: [consents, collections, wealth data]\n  sources: [docs.insurely.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insurely/refs/heads/main/authentication/insurely-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Open Finance
- Insurance
- Fintech
- PSD2
- Financial Data
- Data Aggregation
- Pensions
- Wealth
- Europe
---
