---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Listings API
  slug: listings-api
  spec_type: OpenAPI
  url: https://listingsapi.com/openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Listings Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listings API secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Listings API
provider_slug: listings-api
scheme_count: 3
schemes:
- access_levels:
  - Read
  - Write
  description: 'Authenticate with `Authorization: API <your-key>`.'
  in: header
  name: apiKey
  notes: Header value is the literal "API " prefix plus the key. Keys are created/rotated in the dashboard, one per agent recommended so each can be revoked independently; revocation is immediate. Access level (Read or Write) is chosen at creation. The agent-facing auth guide at https://www.listingsapi.com/auth.md documents the discover-register-credential flow.
  parameter: Authorization
  sources:
  - openapi/listings-api-openapi.yaml
  type: apiKey
- description: RapidAPI marketplace key. Sent with `X-RapidAPI-Host` when calling via the RapidAPI proxy.
  in: header
  name: rapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/listings-api-openapi.yaml
  type: apiKey
- description: RapidAPI marketplace host header. Sent with `X-RapidAPI-Key` when calling via the RapidAPI proxy.
  in: header
  name: rapidApiHost
  parameter: X-RapidAPI-Host
  sources:
  - openapi/listings-api-openapi.yaml
  type: apiKey
slug: listings-api-authentication
source_filename: listings-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/listings-api-openapi.yaml, https://docs.listingsapi.com/docs/authentication, https://www.listingsapi.com/auth.md\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Authenticate with `Authorization: API <your-key>`.'\n  sources:\n  - openapi/listings-api-openapi.yaml\n  access_levels:\n  - Read\n  - Write\n  notes: Header value is the literal \"API \" prefix plus the key. Keys are created/rotated in the dashboard,\n    one per agent recommended so each can be revoked independently; revocation is immediate. Access level\n    (Read or Write) is chosen at creation. The agent-facing auth guide at https://www.listingsapi.com/auth.md\n    documents the discover-register-credential flow.\n- name: rapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: RapidAPI marketplace key. Sent with\
  \ `X-RapidAPI-Host` when calling via the RapidAPI proxy.\n  sources:\n  - openapi/listings-api-openapi.yaml\n- name: rapidApiHost\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Host\n  description: RapidAPI marketplace host header. Sent with `X-RapidAPI-Key` when calling via the RapidAPI\n    proxy.\n  sources:\n  - openapi/listings-api-openapi.yaml\ndocs: https://docs.listingsapi.com/docs/authentication\noauth_note: 'The hosted MCP server additionally accepts OAuth 2.0 Bearer tokens: RFC 8414 metadata at\n  https://listingsapi.com/.well-known/oauth-authorization-server (PKCE S256, dynamic client registration,\n  scopes read/write); consent creates an API key named after the client. See scopes/listings-api-scopes.yml.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/authentication/listings-api-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Business Listings
- Local SEO
- Locations
- Reviews
- Google Business Profile
- Analytics
- citation-management
- Local Marketing
- social-publishing
- MCP
- agent-native
---
