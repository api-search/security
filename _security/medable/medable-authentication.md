---
api_key_in:
- header
auth_types:
- apiKey
- http-signature
- session
description: ''
kind: authentication
layout: security
method: searched
name: Medable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medable secures its APIs with apiKey, http-signature, and session across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medable
provider_slug: medable
scheme_count: 3
schemes:
- csrf: When CSRF protection is enabled on the App, authenticated requests must send the medable-csrf-token header.
  description: Cookie-based session initiated by account registration or login. Times out after a period of inactivity per org settings. Two-factor authentication applies.
  name: SessionAuth
  sources:
  - docs
  type: session
- description: Secure request-signing mechanism for third-party/back-end integrations (e.g. EMR, HL7 messaging appliance). Signing keys can be scoped to single or multiple user accounts and given a timed expiry.
  headers:
  - name: Medable-Client-Key
    value: The API key of the calling App.
  - name: Medable-Client-Signature
    value: The calculated request signature.
  - name: Medable-Client-Timestamp
    value: Client Unix timestamp in milliseconds; the server issues a Medable-Server-Time response header clients can use to synchronize.
  - name: Medable-Client-Nonce
    value: Client-generated nonce matching /^[a-z\d]{16}$/i, used to prevent replay attacks.
  - name: Medable-Client-Account
    value: Optionally sets the calling principal by account id (when the App is configured to allow principal override).
  name: SignatureAuth
  sources:
  - docs
  type: http-signature
- description: Per-App API key generated under Settings > Apps, used together with the signing secret for signature-based calls and to identify the client application.
  in: header
  name: ApiKey
  sources:
  - docs
  type: apiKey
slug: medable-authentication
source_filename: medable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.medable.com/getting-started/cortex-user-guide/authentication.md\ndocs: https://docs.medable.com/getting-started/cortex-user-guide/authentication\nsummary:\n  types:\n  - apiKey\n  - http-signature\n  - session\n  api_key_in:\n  - header\n  notes: >-\n    Cortex uses two authentication models. Session-based authentication (cookies)\n    for interactive client apps (mobile/web) where individual users authenticate\n    with credentials; two-factor authentication applies to sessions. Signature-based\n    authentication for privileged back-end/system integrations, using a signing key\n    (key + secret) issued per App within an org. There is no OAuth2 / OpenID Connect\n    surface. Apps are created under Settings > Apps and expose an API key.\nschemes:\n- name: SessionAuth\n  type: session\n  description: >-\n    Cookie-based session initiated by account registration or login. Times out after\n    a period of inactivity\
  \ per org settings. Two-factor authentication applies.\n  csrf: >-\n    When CSRF protection is enabled on the App, authenticated requests must send the\n    medable-csrf-token header.\n  sources:\n  - docs\n- name: SignatureAuth\n  type: http-signature\n  description: >-\n    Secure request-signing mechanism for third-party/back-end integrations (e.g. EMR,\n    HL7 messaging appliance). Signing keys can be scoped to single or multiple user\n    accounts and given a timed expiry.\n  headers:\n  - name: Medable-Client-Key\n    value: The API key of the calling App.\n  - name: Medable-Client-Signature\n    value: The calculated request signature.\n  - name: Medable-Client-Timestamp\n    value: >-\n      Client Unix timestamp in milliseconds; the server issues a Medable-Server-Time\n      response header clients can use to synchronize.\n  - name: Medable-Client-Nonce\n    value: Client-generated nonce matching /^[a-z\\d]{16}$/i, used to prevent replay attacks.\n  - name: Medable-Client-Account\n\
  \    value: >-\n      Optionally sets the calling principal by account id (when the App is configured\n      to allow principal override).\n  sources:\n  - docs\n- name: ApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-App API key generated under Settings > Apps, used together with the signing\n    secret for signature-based calls and to identify the client application.\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medable/refs/heads/main/authentication/medable-authentication.yml
summary_line: apiKey/http-signature/session · 3 schemes
tags:
- Company
- Human Health
- Clinical Trials
- Life Sciences
- eCOA
- Healthcare
- Decentralized Clinical Trials
- Backend as a Service
- Agentic AI
---
