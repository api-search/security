---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Payengine Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayEngine declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: PayEngine
provider_slug: payengine
scheme_count: 4
schemes:
- description: The private (secret) API key, presented as an HTTP Basic credential. Can make any API call on behalf of the partner account.
  format: 'Authorization: Basic <partner_private_token>'
  handling: Docs state the private key is shown only once at creation and is redacted by the dashboard afterwards - if lost it cannot be recovered and must be rotated. Docs explicitly warn it must be kept out of version control and never exposed client-side.
  header: Authorization
  id: partner_private_key
  in: header
  issued_via: Partner console, Settings > API Keys
  roles_permitted:
  - Admin
  - Developer
  scheme: basic
  type: http
- description: The public key identifies the partner to the browser-side web-component loader and SecureFields JS. Safe to expose client-side; carries no ability to call the REST API.
  format: <loader-url>/js/1.0.0/embed.js?key=<Public API Key>
  id: partner_public_key
  in: query
  name: key
  type: apiKey
- description: A short-lived access token obtained server-side using the partner private key and handed to the browser through a fetchAccessToken callback. Scopes an embedded widget to a single merchant, so the private key never reaches the client.
  docs: https://docs.payengine.co/developer-docs/getting-started-1/securing-embedded-uis-merchant-session
  id: merchant_session_token
  scheme: bearer
  scope_parameter:
    effect: Setting scope to 'readonly' restricts actions inside the embedded widgets - it hides the Refund button in the Transactions widget and disables Export.
    name: scope
    values:
    - readonly
  status: current
  type: http
- algorithm: HMAC-SHA256
  deprecation_note: Docs state HMAC-based security "has been deprecated and will be removed in a future release", and recommend migrating to MerchantSession. Backward compatibility is maintained in the interim. No removal date is published.
  description: Legacy scheme for securing embedded UIs - an HMAC-SHA256 over the merchant id keyed with the partner's private key, generated at user login.
  docs: https://docs.payengine.co/developer-docs/getting-started-1/securing-embedded-uis-merchant-session/securing-embeddable-uis
  id: hmac_web_component_auth
  status: deprecated
  type: hmac
slug: payengine-authentication
source_filename: payengine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.payengine.co/developer-docs/getting-started-1/generate-access-tokens\nname: PayEngine authentication profile\nsummary: >-\n  PayEngine uses a three-credential model rather than a single API key. A private\n  (secret) key authenticates server-to-server REST calls over HTTP Basic; a public key\n  identifies the partner to browser-loaded web components; and a short-lived merchant\n  session access token, minted server-side from the private key, scopes an embedded\n  widget to one merchant. There is no OAuth 2.0 authorization server and no OpenID\n  Connect discovery document on any PayEngine host, so scopes/ is deliberately not\n  emitted for this provider.\nderived_from_openapi: false\nderived_from_openapi_reason: >-\n  PayEngine publishes no public OpenAPI. The API reference at https://docs-api.payengine.co/\n  is behind a \"PayEngine Docs Login\", and the public docs state the spec is \"provided from\n  within\
  \ your partner portal\". This profile was read from the public getting-started and\n  security guides instead.\nschemes:\n- id: partner_private_key\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Authorization: Basic <partner_private_token>'\n  description: >-\n    The private (secret) API key, presented as an HTTP Basic credential. Can make any API\n    call on behalf of the partner account.\n  handling: >-\n    Docs state the private key is shown only once at creation and is redacted by the\n    dashboard afterwards - if lost it cannot be recovered and must be rotated. Docs\n    explicitly warn it must be kept out of version control and never exposed client-side.\n  issued_via: Partner console, Settings > API Keys\n  roles_permitted: [Admin, Developer]\n- id: partner_public_key\n  type: apiKey\n  in: query\n  name: key\n  format: '<loader-url>/js/1.0.0/embed.js?key=<Public API Key>'\n  description: >-\n    The public key identifies the partner to the\
  \ browser-side web-component loader and\n    SecureFields JS. Safe to expose client-side; carries no ability to call the REST API.\n- id: merchant_session_token\n  type: http\n  scheme: bearer\n  description: >-\n    A short-lived access token obtained server-side using the partner private key and\n    handed to the browser through a fetchAccessToken callback. Scopes an embedded widget\n    to a single merchant, so the private key never reaches the client.\n  scope_parameter:\n    name: scope\n    values: [readonly]\n    effect: >-\n      Setting scope to 'readonly' restricts actions inside the embedded widgets - it\n      hides the Refund button in the Transactions widget and disables Export.\n  docs: https://docs.payengine.co/developer-docs/getting-started-1/securing-embedded-uis-merchant-session\n  status: current\n- id: hmac_web_component_auth\n  type: hmac\n  algorithm: HMAC-SHA256\n  description: >-\n    Legacy scheme for securing embedded UIs - an HMAC-SHA256 over the merchant id\
  \ keyed\n    with the partner's private key, generated at user login.\n  status: deprecated\n  deprecation_note: >-\n    Docs state HMAC-based security \"has been deprecated and will be removed in a future\n    release\", and recommend migrating to MerchantSession. Backward compatibility is\n    maintained in the interim. No removal date is published.\n  docs: https://docs.payengine.co/developer-docs/getting-started-1/securing-embedded-uis-merchant-session/securing-embeddable-uis\noauth2: false\nopenid_connect: false\nmutual_tls: false\nmfa:\n  console_2fa: true\n  note: The console permissions matrix lists 2FA as available to Admin, User and Developer roles.\nroles:\n  model: Three fixed console roles gate credential and webhook management.\n  values:\n  - name: Admin\n    api_keys: true\n    webhooks: true\n    embedded_widget: true\n  - name: User\n    api_keys: false\n    webhooks: false\n    embedded_widget: false\n  - name: Developer\n    api_keys: true\n    webhooks: true\n    embedded_widget:\
  \ true\n  docs: https://docs.payengine.co/developer-docs/getting-started-1/2.-user-account-types-and-permissions\nkey_environments:\n  test_prefix: pk_test_\n  note: >-\n    Public test keys are shown in the docs as pk_test_xxx. The docs describe a distinct\n    Sandbox account rather than a prefix-switched key on one account; see\n    sandbox/payengine-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payengine/refs/heads/main/authentication/payengine-authentication.yml
summary_line: 4 schemes
tags:
- Payments
- Embedded Payments
- Payment Facilitation
- Merchant Onboarding
- Payment Gateway
- Financial Services
- ACH
- Tokenization
- Webhooks
- Fintech
- Company
---
