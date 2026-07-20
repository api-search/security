---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Alloovium API
  slug: alloovium-api
  spec_type: OpenAPI
  url: https://api.alloovium.com/api/v2/openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alloovium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Alloovium secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Alloovium
provider_slug: alloovium
scheme_count: 2
schemes:
- format: 'Authorization: Bearer <key>'
  in: header
  key_length: 60
  key_prefixes:
  - ak_live_
  - ak_test_
  name: ApiKeyAuth
  notes: Keys are rejected in query strings, cookies, or JSON bodies — header only. Test and live keys are created in the Developer Console.
  parameter: Authorization
  type: apiKey
- dcr_note: Clients self-register without pre-provisioning; dynamically registered clients are always issued read-only scopes.
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.alloovium.com/api/v2/oauth/authorize
    flow: authorizationCode
    pkce: required (S256)
    registrationUrl: https://api.alloovium.com/api/v2/oauth/register
    revocationUrl: https://api.alloovium.com/api/v2/oauth/revoke
    tokenUrl: https://api.alloovium.com/api/v2/oauth/token
  name: OAuth2
  note: OAuth tokens are not accepted on the MCP transport (API key only there).
  type: oauth2
  version: OAuth 2.1
slug: alloovium-authentication
source_filename: alloovium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.alloovium.com/en/developers/authentication\ndocs: https://www.alloovium.com/en/developers/authentication\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <key>'\n  key_prefixes: [ak_live_, ak_test_]\n  key_length: 60\n  notes: >-\n    Keys are rejected in query strings, cookies, or JSON bodies — header only. Test and live keys are\n    created in the Developer Console.\n- name: OAuth2\n  type: oauth2\n  version: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    pkce: required (S256)\n    authorizationUrl: https://api.alloovium.com/api/v2/oauth/authorize\n    tokenUrl: https://api.alloovium.com/api/v2/oauth/token\n    registrationUrl: https://api.alloovium.com/api/v2/oauth/register\n    revocationUrl: https://api.alloovium.com/api/v2/oauth/revoke\n\
  \  dynamic_client_registration: true\n  dcr_note: >-\n    Clients self-register without pre-provisioning; dynamically registered clients are always issued\n    read-only scopes.\n  note: OAuth tokens are not accepted on the MCP transport (API key only there).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloovium/refs/heads/main/authentication/alloovium-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Construction
- Document Intelligence
- Compliance
- Artificial Intelligence
- Construction Technology
- Documents
- MCP
---
