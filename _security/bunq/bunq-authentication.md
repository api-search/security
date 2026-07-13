---
api_key_in: []
api_specs:
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Session (Handshake) API
  slug: bunq-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq User API
  slug: bunq-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Monetary Account API
  slug: bunq-monetary-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Payment API
  slug: bunq-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Request Inquiry API
  slug: bunq-request-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Card API
  slug: bunq-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Attachment API
  slug: bunq-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Customer Statement (Export) API
  slug: bunq-customer-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Notification Filter (Callbacks) API
  slug: bunq-notification-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: derived
name: Bunq Authentication
name_suffix: Authentication
oauth_flows: []
overview: bunq secures its APIs with apiKey and signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: bunq
provider_slug: bunq
scheme_count: 3
schemes:
- description: Installation token returned by POST /v1/installation. Used only to authenticate the device-server and session-server handshake calls. Obtained by POSTing your 2048-bit RSA (PKCS#8) public key; the response also returns the bunq server_public_key used to verify response signatures.
  headerName: X-Bunq-Client-Authentication
  in: header
  name: installationToken
  sources:
  - openapi/bunq-openapi.yml
  - https://doc.bunq.com/basics/authentication
  type: apiKey
- description: Session token returned by POST /v1/session-server. Sent on every business call for the life of the session. Opening the session requires your bunq API key (the "secret").
  headerName: X-Bunq-Client-Authentication
  in: header
  name: sessionToken
  sources:
  - openapi/bunq-openapi.yml
  - https://doc.bunq.com/quickstart/opening-a-session
  type: apiKey
- algorithm: RSA-SHA256 (PKCS#1 v1.5)
  description: Base64-encoded RSA signature of the request body, created with your private key using SHA-256 and PKCS#1 v1.5 padding. Required on the device-server and session-server handshake calls and, per bunq's signing documentation, on authenticated requests. bunq signs its responses in X-Bunq-Server-Signature, which the client verifies with the installation server_public_key.
  headerName: X-Bunq-Client-Signature
  in: header
  name: clientSignature
  sources:
  - https://doc.bunq.com/basics/signing
  - https://doc.bunq.com/basics/signing/python-code-example
  type: signature
slug: bunq-authentication
source_filename: bunq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/bunq-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - signature\n  note: >-\n    bunq authentication is a multi-step, RSA-signed handshake, not a simple\n    bearer token. An API key is exchanged for a session via installation ->\n    device-server -> session-server, and every request is additionally signed\n    with the client private key.\nschemes:\n- name: installationToken\n  type: apiKey\n  in: header\n  headerName: X-Bunq-Client-Authentication\n  description: >-\n    Installation token returned by POST /v1/installation. Used only to\n    authenticate the device-server and session-server handshake calls. Obtained\n    by POSTing your 2048-bit RSA (PKCS#8) public key; the response also returns\n    the bunq server_public_key used to verify response signatures.\n  sources:\n  - openapi/bunq-openapi.yml\n  - https://doc.bunq.com/basics/authentication\n- name: sessionToken\n  type: apiKey\n  in: header\n  headerName:\
  \ X-Bunq-Client-Authentication\n  description: >-\n    Session token returned by POST /v1/session-server. Sent on every business\n    call for the life of the session. Opening the session requires your bunq API\n    key (the \"secret\").\n  sources:\n  - openapi/bunq-openapi.yml\n  - https://doc.bunq.com/quickstart/opening-a-session\n- name: clientSignature\n  type: signature\n  in: header\n  headerName: X-Bunq-Client-Signature\n  algorithm: RSA-SHA256 (PKCS#1 v1.5)\n  description: >-\n    Base64-encoded RSA signature of the request body, created with your private\n    key using SHA-256 and PKCS#1 v1.5 padding. Required on the device-server and\n    session-server handshake calls and, per bunq's signing documentation, on\n    authenticated requests. bunq signs its responses in X-Bunq-Server-Signature,\n    which the client verifies with the installation server_public_key.\n  sources:\n  - https://doc.bunq.com/basics/signing\n  - https://doc.bunq.com/basics/signing/python-code-example\n\
  notes: >-\n  API keys for production are issued in the bunq mobile app; sandbox keys are\n  issued via the developer portal or the sandbox tinker/hackathon toolkit. PSD2\n  third parties register an eIDAS certificate to obtain a\n  UserPaymentServiceProvider and API key. bunq also supports OAuth for\n  third-party access on top of this model.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/authentication/bunq-authentication.yml
summary_line: apiKey/signature · 3 schemes
tags:
- Banking
- Neobank
- Payments
- Accounts
- SEPA
- Open Banking
- Fintech
- Europe
- Netherlands
---
