---
api_key_in:
- header
api_specs:
- filename: whisperr-inc-runtime-openapi.json
  format: json
  label: Whisperr Runtime API
  slug: whisperr-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisperr-inc/refs/heads/main/openapi/whisperr-inc-runtime-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Whisperr Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whisperr, Inc. secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Whisperr, Inc.
provider_slug: whisperr-inc
scheme_count: 3
schemes:
- alternate_parameter: X-API-Key
  applies_to:
  - trackEvent
  - trackEventBatch
  - identifyUser
  - getUser
  - getUserState
  - previewDecision
  description: 'App ingestion key. Either `X-API-Key: wrk_...` or `Authorization: Bearer wrk_...` is accepted — the OpenAPI declares only the latter.'
  in: header
  issuance: Whisperr dashboard, Developer -> API Keys
  key_prefix: wrk_
  management_operations:
  - listDashboardAPIKeys
  - createDashboardAPIKey
  - deleteDashboardAPIKey
  name: APIKey
  parameter: Authorization
  publishable: true
  publishable_note: Documented as publishable — it ships in client bundles (browser, React Native, Flutter, Swift SDKs all take it directly). The provider's own analogy is a PostHog project key, not a secret. Do not treat a leaked wrk_ key as a credential incident; do rotate it via the dashboard if abused.
  scope_of_access: Ingest events and identify users for ONE app, plus read that app's users and preview decisions. It cannot read another app's data.
  sources:
  - https://docs.whisperr.net/api/overview/
  - openapi/whisperr-inc-runtime-openapi.json
  type: apiKey
- bearerFormat: Supabase JWT
  description: 'Use `Authorization: Bearer <supabase_access_token>` from Supabase Auth.'
  identity_provider: Supabase Auth
  name: DashboardBearer
  note: Guards all 44 dashboard operations. This is a human console session token, not a machine credential — there is no documented service-account or client-credentials flow to obtain one, so the dashboard surface is not programmatically accessible by design.
  scheme: bearer
  sources:
  - openapi/whisperr-inc-runtime-openapi.json
  type: http
- description: Shared secret guarding the internal onboarding import.
  in: header
  name: OnboardingImportSecret
  note: Internal service-to-service only (importOnboardingSession) — whisp-onboarding-panel handing a completed session to the whisp-go runtime. Not available to customers.
  parameter: X-Whisp-Onboarding-Import-Secret
  sources:
  - openapi/whisperr-inc-runtime-openapi.json
  type: apiKey
slug: whisperr-inc-authentication
source_filename: whisperr-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.whisperr.net/api/overview/ (Authentication section) and\n  https://github.com/WhisperrAI/whisperr-spec/blob/main/SPEC.md, reconciled\n  against openapi/whisperr-inc-runtime-openapi.json\ndocs: https://docs.whisperr.net/api/overview/\nnote: >-\n  Upgraded from derived to searched. The served OpenAPI documents only\n  `Authorization: Bearer` for the ingestion key; the provider's documentation and\n  wire spec both state that `X-API-Key` is equally accepted, and name the key\n  prefix and its publishable nature. That information exists only in prose, so\n  the spec alone understates the auth model.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  primary: >-\n    Publishable per-app ingestion API key (wrk_ prefix) for the six public\n    operations. Everything else is a human console session.\nschemes:\n- name: APIKey\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization\n  alternate_parameter: X-API-Key\n  key_prefix: wrk_\n  publishable: true\n  description: >-\n    App ingestion key. Either `X-API-Key: wrk_...` or `Authorization: Bearer\n    wrk_...` is accepted — the OpenAPI declares only the latter.\n  issuance: Whisperr dashboard, Developer -> API Keys\n  management_operations:\n  - listDashboardAPIKeys\n  - createDashboardAPIKey\n  - deleteDashboardAPIKey\n  scope_of_access: >-\n    Ingest events and identify users for ONE app, plus read that app's users and\n    preview decisions. It cannot read another app's data.\n  publishable_note: >-\n    Documented as publishable — it ships in client bundles (browser, React\n    Native, Flutter, Swift SDKs all take it directly). The provider's own analogy\n    is a PostHog project key, not a secret. Do not treat a leaked wrk_ key as a\n    credential incident; do rotate it via the dashboard if abused.\n  applies_to:\n  - trackEvent\n  - trackEventBatch\n\
  \  - identifyUser\n  - getUser\n  - getUserState\n  - previewDecision\n  sources:\n  - https://docs.whisperr.net/api/overview/\n  - openapi/whisperr-inc-runtime-openapi.json\n- name: DashboardBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Supabase JWT\n  description: 'Use `Authorization: Bearer <supabase_access_token>` from Supabase Auth.'\n  identity_provider: Supabase Auth\n  note: >-\n    Guards all 44 dashboard operations. This is a human console session token,\n    not a machine credential — there is no documented service-account or\n    client-credentials flow to obtain one, so the dashboard surface is not\n    programmatically accessible by design.\n  sources:\n  - openapi/whisperr-inc-runtime-openapi.json\n- name: OnboardingImportSecret\n  type: apiKey\n  in: header\n  parameter: X-Whisp-Onboarding-Import-Secret\n  description: Shared secret guarding the internal onboarding import.\n  note: >-\n    Internal service-to-service only (importOnboardingSession) — whisp-onboarding-panel\n\
  \    handing a completed session to the whisp-go runtime. Not available to\n    customers.\n  sources:\n  - openapi/whisperr-inc-runtime-openapi.json\nunauthenticated:\n- path: /health\n  operationId: getHealth\n  verified: probed 2026-08-13, HTTP 200\n- path: /metrics\n  operationId: getMetrics\n  verified: probed 2026-08-13, HTTP 200\n- path: /openapi.json\n  verified: probed 2026-08-13, HTTP 200\n- path: /delivery/webhooks/postmark/{token}\n  operationId: receivePostmarkDeliveryWebhook\n  note: Authenticated by the unguessable token in the path; inbound from Postmark.\nobserved_failure:\n  method: probed\n  request: GET https://api.whisperr.net/v1/users/test (no credentials)\n  status: 401\n  body: '{\"error\":{\"code\":\"missing_api_key\",\"message\":\"api key is required\",\"request_id\":\"<uuid>\"}}'\n  note: Confirms the key is genuinely enforced on the public surface.\ngaps:\n- No OAuth 2.0, OpenID Connect, or mTLS anywhere in the API.\n- No scopes or permissions model — the ingestion\
  \ key is all-or-nothing for its app.\n- No documented key rotation or expiry policy.\n- >-\n  No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n  on any host (probed 2026-08-13: 404 on api.whisperr.net).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisperr-inc/refs/heads/main/authentication/whisperr-inc-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Customer Retention
- Churn
- Marketing Automation
- Artificial Intelligence
- SaaS
- Subscription
- Customer Engagement
- Event Ingestion
- Analytics
- Customer Data
- Email Delivery
- Agents
---
