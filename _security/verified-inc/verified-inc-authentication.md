---
anonymous_access: false
api_key_in: []
api_specs:
- filename: verified-inc-openapi-generated.yml
  format: yaml
  label: Verified API
  slug: verified-inc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verified-inc/openapi/_ae-authored/verified-inc-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Verified Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verified declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Verified
provider_slug: verified-inc
scheme_count: 2
schemes:
- description: Requests to authenticated Verified API endpoints require an API key as an `Authorization` header value (_without_ a `Bearer` prefix).
  header: Authorization
  in: header
  name: apiKey
  scope: Each API key is specific to a brand and an environment (Sandbox or Production); keys are managed in the Verified Dashboard.
  server_side_only: true
  type: apiKey
- description: Client SDK flows use a session key that your server obtains via POST /client/1-click and passes to new VerifiedClientSdk({sessionKey}).
  docs: https://docs.verified.inc/reference/sdk/methods
  name: sessionKey
  type: session-token
slug: verified-inc-authentication
source_filename: verified-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://docs.verified.inc/reference/api/authentication\ndocs: https://docs.verified.inc/reference/api/authentication\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  description: Requests to authenticated Verified API endpoints require an API key as an `Authorization` header value (_without_ a `Bearer` prefix).\n  scope: Each API key is specific to a brand and an environment (Sandbox or Production); keys are managed in the Verified Dashboard.\n  server_side_only: true\n- name: sessionKey\n  type: session-token\n  description: Client SDK flows use a session key that your server obtains via POST /client/1-click and passes to new VerifiedClientSdk({sessionKey}).\n  docs: https://docs.verified.inc/reference/sdk/methods\nnotes:\n- Using an API key client side is blocked by the firewall with HTTP 418.\n- 'Webhook (1-Click Health) requests are signed: X-Webhook-Signature v1=HMAC-SHA256(secret, `${timestamp}.${rawBody}`),\
  \ with X-Webhook-Timestamp; receiver auth can be None, API Key or Basic Auth.'\noauth: false\n"
source_yaml_url: https://artifacts.apis.io/verified-inc/authentication/verified-inc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Identity Verification
- Onboarding
- Phone Verification
- KYC
- Autofill
- Health Insurance
- Fintech
---
