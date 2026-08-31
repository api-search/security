---
api_key_in:
- header
api_specs:
- filename: moonscale-liveavatar-api-openapi.yml
  format: yaml
  label: Moonscale Live Avatar API
  slug: moonscale-liveavatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/openapi/moonscale-liveavatar-api-openapi.yml
- filename: moonscale-videogeneration-api-openapi.yml
  format: yaml
  label: Moonscale Video Generation API
  slug: moonscale-videogeneration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/openapi/moonscale-videogeneration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moonscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moonscale secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moonscale
provider_slug: moonscale
scheme_count: 1
schemes:
- applied: global
  in: header
  name: ApiKeyAuth
  note: 'Declared in the root security[] block AND repeated as an operation-level security[] on both /api/studio-avatar/* operations. Verified live: an unauthenticated GET to https://api-prd.moonscale.com/health returns HTTP 401 {"message":"Unauthorized request. No API key provided."}'
  parameter: x-api-key
  sources:
  - openapi/moonscale-openapi-original.json
  type: apiKey
slug: moonscale-authentication
source_filename: moonscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/moonscale-openapi-original.json\ndocs: https://vidlab7-d7584a5d.mintlify.app/api-reference/endpoint/createApiKey\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Single-scheme API. Every operation in the published OpenAPI is protected by one\n    apiKey scheme carried in the x-api-key request header. There is no OAuth 2.0,\n    OpenID Connect, HTTP basic/bearer or mTLS surface, so scopes/ is intentionally\n    not emitted for this provider.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applied: global\n  sources: [openapi/moonscale-openapi-original.json]\n  note: >-\n    Declared in the root security[] block AND repeated as an operation-level security[]\n    on both /api/studio-avatar/* operations. Verified live: an unauthenticated GET to\n    https://api-prd.moonscale.com/health returns HTTP 401\n    {\"message\":\"Unauthorized request.\
  \ No API key provided.\"}\nkey_issuance:\n  self_service: false\n  where: https://app.moonscale.com  (Moonscale Studio -> API, bottom of the left sidebar)\n  steps:\n  - Sign in to Moonscale Studio at app.moonscale.com\n  - Open the API section at the bottom-left of the sidebar\n  - Click \"Generate new key\", name the key, click \"Generate\"\n  - Copy the key immediately — it is shown once and permanently hidden afterwards\n  rotation: >-\n    No rotate operation is published. The documented recovery for a lost key is to delete\n    it and generate a new one.\n  gate: >-\n    Moonscale's own documentation states API access is feature-flagged and may not be\n    enabled for an account; accounts without the API section are told to email\n    support@moonscale.com to request access. Key issuance is therefore account-gated and\n    not self-service, even though the reference and the OpenAPI are public.\n  contact: support@moonscale.com\ntransport:\n  https_only: true\n  observed_headers:\n\
  \  - {header: x-request-id, note: returned on every response; correlation id for support}\n  - {header: server, value: Google Frontend}\nevidence:\n- {url: 'https://api-prd.moonscale.com/health', status: 401, body: '{\"message\":\"Unauthorized request. No API key provided.\"}'}\n- {url: 'https://api-prd.moonscale.com/api/v1/avatars', status: 403, body: '{\"message\":\"Forbidden\"}'}\n- {url: 'https://vidlab7-d7584a5d.mintlify.app/api-reference/openapi.json', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/authentication/moonscale-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Automation
- Lead Generation
- AI Agents
- Conversational AI
- CRM
- Video Generation
- Avatars
- Speech
- Germany
---
