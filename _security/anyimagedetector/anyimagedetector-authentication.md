---
api_key_in:
- header
api_specs:
- filename: anyimagedetector-detection-api-openapi.yml
  format: yaml
  label: AnyImageDetector Detection API
  slug: anyimagedetector-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anyimagedetector/refs/heads/main/openapi/anyimagedetector-detection-api-openapi.yml
auth_types:
- http-bearer
- apiKey
description: AnyImageDetector uses a single static API key, presented either as an HTTP Bearer token or in an x-api-key header. There is no OAuth, no OpenID Connect, no mTLS, no scopes, no refresh and no token exchange — the key is the whole authorization model, and entitlement is enforced by plan and credit balance rather than by scope.
kind: authentication
layout: security
method: searched
name: Anyimagedetector Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnyImageDetector secures its APIs with http-bearer and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AnyImageDetector
provider_slug: anyimagedetector
scheme_count: 2
schemes:
- description: Pass the API key as a Bearer token in the Authorization header. Documented as the primary method.
  in: header
  key_prefix: sk_
  name: BearerAuth
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://imagedetector.online/docs
  type: http
  value_format: Bearer sk_your_api_key
- description: Alternative to the Authorization header. The docs state to provide ONE of the two, not both.
  in: header
  key_prefix: sk_
  name: ApiKeyHeader
  parameter_name: x-api-key
  sources:
  - https://imagedetector.online/docs
  type: apiKey
  value_format: sk_your_api_key
slug: anyimagedetector-authentication
source_filename: anyimagedetector-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://imagedetector.online/docs\ndocs: https://imagedetector.online/docs\ndescription: >-\n  AnyImageDetector uses a single static API key, presented either as an HTTP Bearer token or in\n  an x-api-key header. There is no OAuth, no OpenID Connect, no mTLS, no scopes, no refresh and\n  no token exchange — the key is the whole authorization model, and entitlement is enforced by\n  plan and credit balance rather than by scope.\nsummary:\n  types: [http-bearer, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  openid_connect: false\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    parameter_name: Authorization\n    value_format: 'Bearer sk_your_api_key'\n    key_prefix: sk_\n    description: >-\n      Pass the API key as a Bearer token in the Authorization header. Documented as the primary\n      method.\n    sources: [https://imagedetector.online/docs]\n\
  \  - name: ApiKeyHeader\n    type: apiKey\n    in: header\n    parameter_name: x-api-key\n    value_format: 'sk_your_api_key'\n    key_prefix: sk_\n    description: >-\n      Alternative to the Authorization header. The docs state to provide ONE of the two, not\n      both.\n    sources: [https://imagedetector.online/docs]\nkey_management:\n  issued_at: Settings -> API Keys (signed-in account UI)\n  self_service: true\n  eligibility: >-\n    A paid plan is required. The docs state plainly that free accounts and unauthenticated\n    guests cannot create API keys or call /v1 endpoints.\n  shown_once: true\n  rotation_policy: not published\n  expiration: not published\n  revocation: not published\nfailure_modes:\n  - status: 401\n    error: unauthorized\n    condition: Missing or invalid API key.\n    observed_body: '{\"error\":\"unauthorized\",\"message\":\"Missing API key\"}'\n  - status: 403\n    error: paid_plan_required\n    condition: Valid key on an account without a paid plan.\n \
  \ - status: 402\n    error: insufficient_credits\n    condition: Authenticated but out of credits.\ntransport:\n  https_only: true\n  note: The docs state all endpoints are served over HTTPS and versioned with a /v1 prefix.\nx-evidence:\n  probed: '2026-08-11'\n  url: https://imagedetector.online/v1/image/detect\n  http_status: 401\n  content_type: application/json\n  note: >-\n    Anonymous POST returned the documented 401 unauthorized envelope, confirming the key is\n    required and enforced at the edge.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyimagedetector/refs/heads/main/authentication/anyimagedetector-authentication.yml
summary_line: http-bearer/apiKey · 2 schemes
tags:
- AI image detection
- Image Analysis
- Computer-Vision
- Content Moderation
- Trust and Safety
- Fact Checking
- media verification
- Developer Tools
- Synthetic Media
- Fraud Prevention
---
