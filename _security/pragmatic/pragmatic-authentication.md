---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Pragmatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pragmatic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pragmatic
provider_slug: pragmatic
scheme_count: 1
schemes:
- confidence: medium
  description: The portal bundle sends an Authorization header on authenticated calls and stores a validated token (a users/validate-token/ route exists). The exact token format is not published and could not be observed without credentials.
  evidence: portal bundle references "authorization" header handling and a users/validate-token/ route
  id: portal-session
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: pragmatic-authentication
source_filename: pragmatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://portal.pragmaticsemi.com/static/js/main.88bcd9f5.js - the Pragmatic Customer Portal's\n  own first-party JavaScript bundle, served from Pragmatic's domain; plus live unauthenticated\n  probes of https://api-portal.pragmaticsemi.com/.\ndocs: null\ndocs_note: >-\n  Pragmatic publishes no authentication documentation. There is no developer portal, no API\n  reference and no OpenAPI securitySchemes to derive from, so this profile is assembled ONLY\n  from routes the provider itself ships in its portal bundle and from status codes observed\n  on live unauthenticated requests. Nothing here is inferred beyond what was observed.\napi: pragmatic:customer-portal-api\nbase_url: https://api-portal.pragmaticsemi.com/v1/\npublic_signup: false\naccess: customer-only\nschemes:\n- id: portal-session\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  description: >-\n    The portal bundle sends an Authorization\
  \ header on authenticated calls and stores a\n    validated token (a users/validate-token/ route exists). The exact token format is not\n    published and could not be observed without credentials.\n  confidence: medium\n  evidence: portal bundle references \"authorization\" header handling and a users/validate-token/ route\nmfa:\n  supported: true\n  factors:\n  - totp\n  - recovery-codes\n  evidence: >-\n    The portal bundle ships routes users/totp/create/, users/totp/login/, users/totp/login-update/,\n    users/totp/update/, auth/otpVerification and auth/recoveryCodeLogin - a TOTP enrolment and\n    verification flow with recovery-code fallback.\n  confidence: high\nobserved_routes:\n- path: /v1/auth/login/\n  observed: GET returned 405 Method Not Allowed with a JSON envelope, confirming the route exists and is POST-only\n  status: 405\n- path: /auth/login/\n  observed: 404 - the unversioned prefix is not routed; /v1/ is the live prefix\n  status: 404\naccount_protection:\n  ip_blocking:\
  \ true\n  evidence: portal bundle ships auth/blocked-ips/ and auth/unblock-ip/ administrative routes\npassword_flows:\n- users/forgot-password/\n- users/reset-password/\n- users/set-password/\n- users/change-password/\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\nnotes: >-\n  No OAuth 2.0 or OpenID Connect surface exists: /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server return 404 on api-portal.pragmaticsemi.com and are\n  unreachable behind the captcha on www.pragmaticsemi.com. No API-key issuance is documented\n  anywhere on the public site. This is a human-facing customer portal login, not a\n  programmatic credential surface an agent can obtain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pragmatic/refs/heads/main/authentication/pragmatic-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Semiconductors
- Hardware
- Manufacturing
- Flexible Electronics
- Integrated Circuits
- Foundry
- NFC
- RFID
- Internet of Things
- United Kingdom
---
