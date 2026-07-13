---
api_key_in: []
api_specs:
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Start Verification API
  slug: sinch-verify-start-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Report Verification API
  slug: sinch-verify-report-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
- filename: sinch-verify-openapi.yml
  format: yaml
  label: Sinch Verification Status API
  slug: sinch-verify-verification-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/openapi/sinch-verify-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sinch Verify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sinch Verification API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sinch Verification API
provider_slug: sinch-verify
scheme_count: 2
schemes:
- description: Application-signed request (recommended for production). The Authorization header is "Application {application_key}:{signature}", where signature is a Base64-encoded HMAC-SHA256 computed over a canonicalized string built from the HTTP verb, Content-Type, a Content-MD5 of the body, the x-timestamp header, and the request path, signed with the Base64-decoded application secret. The application key and secret are created and managed in the Sinch Build dashboard. Because signing happens server-to-server, the secret is never exposed to the client.
  headerName: Authorization
  in: header
  name: applicationSigned
  scheme: application-signed
  sources:
  - https://developers.sinch.com/docs/verification/api-reference/authentication/application-signed-request
  type: apiKey
- description: HTTP Basic authentication using the application key as the username and the application secret as the password. Simple to set up and recommended only for prototyping; use application-signed requests in production.
  name: basicAuth
  scheme: basic
  sources:
  - https://developers.sinch.com/docs/verification/api-reference/authentication/basic-authentication
  type: http
slug: sinch-verify-authentication
source_filename: sinch-verify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: https://developers.sinch.com/docs/verification/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: applicationSigned\n  type: apiKey\n  in: header\n  headerName: Authorization\n  scheme: application-signed\n  description: >-\n    Application-signed request (recommended for production). The Authorization\n    header is \"Application {application_key}:{signature}\", where signature is a\n    Base64-encoded HMAC-SHA256 computed over a canonicalized string built from\n    the HTTP verb, Content-Type, a Content-MD5 of the body, the x-timestamp\n    header, and the request path, signed with the Base64-decoded application\n    secret. The application key and secret are created and managed in the Sinch\n    Build dashboard. Because signing happens server-to-server, the secret is\n    never exposed to the client.\n  sources:\n  - https://developers.sinch.com/docs/verification/api-reference/authentication/application-signed-request\n\
  - name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication using the application key as the username and the\n    application secret as the password. Simple to set up and recommended only\n    for prototyping; use application-signed requests in production.\n  sources:\n  - https://developers.sinch.com/docs/verification/api-reference/authentication/basic-authentication\nnotes: >-\n  Both schemes are server-to-server. The Verification API is intended to be\n  called from your backend (or via the Sinch mobile/web Verification SDKs);\n  secrets should never be embedded in client applications. Verification result\n  callbacks can additionally be signed by Sinch so your callback endpoint can\n  validate authenticity.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinch-verify/refs/heads/main/authentication/sinch-verify-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Number Verification
- Phone Verification
- OTP
- 2FA
- CPaaS
- SMS Verification
- Flash Call
- Two-Factor Authentication
- Identity Verification
- Sinch
---
