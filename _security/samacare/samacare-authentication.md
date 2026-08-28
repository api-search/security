---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Samacare Authentication
name_suffix: Authentication
oauth_flows: []
overview: SamaCare declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SamaCare
provider_slug: samacare
scheme_count: 1
schemes:
- error_envelope: '{"error":{"code":"UNAUTHORIZED","message":"Missing Authorization header"}}'
  evidence: 'WWW-Authenticate: Bearer error="invalid_token", error_description="Missing Authorization header"'
  header: Authorization
  id: bearerAuth
  in: header
  scheme: bearer
  status_on_missing_credential: 401
  type: http
slug: samacare-authentication
source_filename: samacare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  live HTTP probes of https://api.samacare.com (root, /docs, /graphql, /openapi.json,\n  /.well-known/*) — 2026-08-26\nnote: >-\n  Derived from the live challenge, not from a published contract: SamaCare publishes no\n  OpenAPI, no auth reference and no developer portal. Every path on api.samacare.com,\n  without exception, returns HTTP 401 with an RFC 6750 Bearer challenge. The scheme below\n  is what the server itself asserts; the token issuance flow (authorization server,\n  grant type, scopes, lifetime) is NOT observable anonymously and is NOT recorded here.\ndocs: null\nschemes:\n- id: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  evidence: >-\n    WWW-Authenticate: Bearer error=\"invalid_token\",\n    error_description=\"Missing Authorization header\"\n  error_envelope: '{\"error\":{\"code\":\"UNAUTHORIZED\",\"message\":\"Missing Authorization header\"}}'\n  status_on_missing_credential:\
  \ 401\noauth2_metadata:\n  authorization_server_discovered: false\n  probes:\n  - url: https://api.samacare.com/.well-known/oauth-authorization-server\n    status: 401\n  - url: https://api.samacare.com/.well-known/openid-configuration\n    status: 401\n  - url: https://www.samacare.com/.well-known/openid-configuration\n    status: 404\n  note: >-\n    The Bearer challenge is RFC 6750 shaped, but no authorization-server metadata document\n    is reachable anonymously, so we cannot confirm whether tokens are issued by an OAuth 2.0\n    authorization server or are opaque partner-issued API tokens. Recorded as unknown rather\n    than guessed.\nonboarding:\n  self_serve: false\n  how_access_is_obtained: >-\n    Through an EHR/EMR/RCM partnership or a customer agreement arranged via\n    https://samacare.com/contact-us — there is no public key issuance, signup-for-an-API\n    flow, or sandbox.\nserver:\n  x_powered_by: Express\n  x_content_type_options: nosniff\n  tls_version: TLSv1.3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samacare/refs/heads/main/authentication/samacare-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- Health Care
- Prior Authorization
- Patient Access
- Specialty Pharmacy
- Life Sciences
- Electronic Health Records
- Revenue Cycle Management
- Market Access
- Artificial Intelligence
---
