---
api_key_in:
- header
api_specs:
- filename: spotdraft-openapi.yml
  format: yaml
  label: SpotDraft Public API
  slug: spotdraft-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotdraft/refs/heads/main/openapi/spotdraft-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spotdraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpotDraft secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SpotDraft
provider_slug: spotdraft
scheme_count: 6
schemes:
- description: Public clickwrap identifier header.
  in: header
  name: ClickwrapId
  parameter: clickwrap-id
  sources:
  - openapi/spotdraft-openapi.yml
  type: apiKey
- in: header
  name: ClientId
  parameter: client-id
  sources:
  - openapi/spotdraft-openapi.yml
  type: apiKey
- in: header
  name: ClientSecret
  parameter: client-secret
  sources:
  - openapi/spotdraft-openapi.yml
  type: apiKey
- description: HTTP Basic auth for supported native integrations. Send base64(client_id:client_secret) in the Authorization header.
  name: NativeIntegrationBasic
  scheme: basic
  sources:
  - openapi/spotdraft-openapi.yml
  type: http
- bearerFormat: JWT
  description: OAuth 2.0 bearer token for workspace user access.
  name: OAuthBearer
  scheme: bearer
  sources:
  - openapi/spotdraft-openapi.yml
  type: http
- description: Browser origin header used for clickwrap domain validation.
  in: header
  name: Origin
  parameter: Origin
  sources:
  - openapi/spotdraft-openapi.yml
  type: apiKey
slug: spotdraft-authentication
source_filename: spotdraft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spotdraft-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ClickwrapId\n  type: apiKey\n  in: header\n  parameter: clickwrap-id\n  description: Public clickwrap identifier header.\n  sources:\n  - openapi/spotdraft-openapi.yml\n- name: ClientId\n  type: apiKey\n  in: header\n  parameter: client-id\n  sources:\n  - openapi/spotdraft-openapi.yml\n- name: ClientSecret\n  type: apiKey\n  in: header\n  parameter: client-secret\n  sources:\n  - openapi/spotdraft-openapi.yml\n- name: NativeIntegrationBasic\n  type: http\n  scheme: basic\n  description: HTTP Basic auth for supported native integrations. Send base64(client_id:client_secret)\n    in the Authorization header.\n  sources:\n  - openapi/spotdraft-openapi.yml\n- name: OAuthBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token for workspace user access.\n  sources:\n  - openapi/spotdraft-openapi.yml\n\
  - name: Origin\n  type: apiKey\n  in: header\n  parameter: Origin\n  description: Browser origin header used for clickwrap domain validation.\n  sources:\n  - openapi/spotdraft-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotdraft/refs/heads/main/authentication/spotdraft-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Contract Lifecycle Management
- CLM
- Contracts
- Legal Tech
- E-Signature
- Clickwrap
- Workflows
- Approvals
- Negotiation
- Templates
- Counterparties
- Obligations
- Analytics
- Webhooks
- AI
- SaaS
- Bangalore
---
