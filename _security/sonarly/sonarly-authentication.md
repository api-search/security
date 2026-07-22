---
api_key_in:
- header
api_specs:
- filename: sonarly-openapi.yml
  format: yaml
  label: Sonarly API
  slug: sonarly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonarly/refs/heads/main/openapi/sonarly-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sonarly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonarly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sonarly
provider_slug: sonarly
scheme_count: 1
schemes:
- description: Bearer token in the Authorization header. For the read-only public API this is a tenant-scoped read-only key with prefix sk_live_ (minted once via POST /api/setup/api-key, returned exactly once). For the setup-session API it is a short-lived (~30 min) setup-scoped token from GET /api/setup/{setup_id}/status, scoped to that one new tenant's setup endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sonarly-openapi.yml
  type: http
slug: sonarly-authentication
source_filename: sonarly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sonarly-openapi.yml\ndocs: https://sonarly.com/docs/public-api\ndetail_source: https://sonarly.com/llms.txt\nsummary:\n  types:\n  - http\n  api_key_in: [header]\n  human_oauth: true\n  notes: >-\n    Two token surfaces, both carried as Authorization: Bearer. Human sign-in and\n    third-party connections use OAuth browser flows; agent/API access uses\n    bearer tokens.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token in the Authorization header. For the read-only public API this\n    is a tenant-scoped read-only key with prefix sk_live_ (minted once via POST\n    /api/setup/api-key, returned exactly once). For the setup-session API it is\n    a short-lived (~30 min) setup-scoped token from GET\n    /api/setup/{setup_id}/status, scoped to that one new tenant's setup\n    endpoints.\n  sources:\n  - openapi/sonarly-openapi.yml\ntoken_types:\n- prefix: sks_setup_\n  name:\
  \ Setup-scoped token\n  lifetime: ~30 minutes\n  scope: single tenant's setup endpoints only\n  issued_by: GET /api/setup/{setup_id}/status once state=authorized\n- prefix: sk_live_\n  name: Public API key\n  lifetime: long-lived\n  scope: read-only, tenant-scoped\n  issued_by: POST /api/setup/api-key (returned exactly once)\n- prefix: whsec_\n  name: Webhook signing secret\n  usage: HMAC-SHA256 signature verification of inbound webhook envelopes\n  issued_by: POST /api/setup/webhook-endpoint (returned exactly once)\noauth_flows:\n  description: >-\n    Human-consent OAuth/browser flows handed off during onboarding; not part of\n    the machine token surface.\n  providers:\n  - {provider: google, purpose: user sign-in / tenant creation}\n  - {provider: github, purpose: user sign-in / tenant creation}\n  - {provider: github-app, purpose: code host connection (Sonarly GitHub App install)}\n  - {provider: sentry, purpose: error tracker connection (OAuth)}\n  - {provider: slack, purpose: notifications\
  \ (OAuth)}\n  - {provider: discord, purpose: notifications (bot invite)}\n  - {provider: linear, purpose: issue tracker (OAuth)}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonarly/refs/heads/main/authentication/sonarly-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Reliability
- Observability
- Monitoring
- Bug Detection
- Incident Management
- Root Cause Analysis
- AI Agents
- Developer Tools
- DevOps
---
