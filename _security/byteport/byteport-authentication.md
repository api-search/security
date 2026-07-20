---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Byteport Authentication
name_suffix: Authentication
oauth_flows: []
overview: Byteport secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Byteport
provider_slug: byteport
scheme_count: 2
schemes:
- bearer_format: Byteport API key (bp_ prefix, 64-char hex secret)
  example: 'Authorization: Bearer [example key]'
  header: Authorization
  name: bearerApiKey
  scheme: bearer
  sources:
  - https://docs.byteport.com/api-reference
  type: http
- description: Mandatory on every request; missing User-Agent returns HTTP 403.
  in: header
  name: User-Agent
  required: true
  sources:
  - https://docs.byteport.com/api-reference
  type: apiKey
slug: byteport-authentication
source_filename: byteport-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.byteport.com/api-reference\ndocs: https://docs.byteport.com/api-reference\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Every request requires two headers. Authorization carries a workspace-scoped bearer\n    API key (prefix bp_) created via POST /v1/tokens or the dashboard; a User-Agent header\n    is mandatory and requests without it are rejected with 403. There are no OAuth2 flows\n    and no granular scopes - keys inherit workspace-level access.\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearer_format: Byteport API key (bp_ prefix, 64-char hex secret)\n  header: Authorization\n  example: 'Authorization: Bearer [example key]'\n  sources: [https://docs.byteport.com/api-reference]\n- name: userAgent\n  type: apiKey\n  in: header\n  name: User-Agent\n  required: true\n  description: Mandatory on every request; missing User-Agent returns HTTP 403.\n\
  \  sources: [https://docs.byteport.com/api-reference]\nkey_management:\n  create_operation: POST /v1/tokens\n  fields: [name, expires_at]\n  token_returned_once: true\n  storage: Byteport stores only a SHA-256 hash of the token; the secret cannot be recovered.\n  expiry: expires_at optional (RFC 3339); omit for non-expiring keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byteport/refs/heads/main/authentication/byteport-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- File Transfer
- Data Transfer
- Acceleration
- Cloud Storage
- Robotics
- Artificial Intelligence
- Satellite
- Infrastructure
- Y Combinator
---
