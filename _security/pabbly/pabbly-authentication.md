---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pabbly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pabbly declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Pabbly
provider_slug: pabbly
scheme_count: 6
schemes:
- api: pabbly:pabbly-subscriptions
  credential_source: Pabbly dashboard -> Settings -> API Settings -> Generate the Keys
  credentials:
  - name: API Key
    role: basic username
  - name: Secret Key
    role: basic password
  docs: https://apidocs.pabbly.com/subscription-billing/reference/guides/authentication
  format: Basic <base64(API_KEY:SECRET_KEY)>
  header: Authorization
  id: subscription-billing-basic
  in: header
  rotation: Regenerate from Settings -> API Settings -> Generate the Keys
  scheme: basic
  type: http
- api: pabbly:pabbly-hook
  credential_source: Pabbly dashboard -> Settings -> API Settings -> Generate the Keys
  docs: https://apidocs.pabbly.com/hook/reference/guides/authentication
  format: Basic <base64(API_KEY:SECRET_KEY)>
  header: Authorization
  id: hook-basic
  in: header
  scheme: basic
  type: http
- api: pabbly:pabbly-email-verification
  credential_source: Pabbly dashboard -> Settings -> API -> Generate API Keys
  docs: https://apidocs.pabbly.com/email-verification/reference/guides/authentication
  format: Basic <base64(API_KEY:SECRET_KEY)>
  header: Authorization
  id: email-verification-basic
  in: header
  scheme: basic
  type: http
- api: pabbly:pabbly-chatflow
  credential_source: Pabbly Chatflow -> Settings -> API & Webhooks
  credentials:
  - name: API key
    role: bearer token
  docs: https://apidocs.pabbly.com/chatflow/reference/guides/authentication
  format: Bearer <API_KEY>
  header: Authorization
  id: chatflow-bearer
  in: header
  scheme: bearer
  type: http
- api: pabbly:pabbly-email-marketing
  docs: https://apidocs.pabbly.com/email-marketing/reference/guides/authentication
  format: Bearer <API_KEY>
  header: Authorization
  id: email-marketing-bearer
  in: header
  scheme: bearer
  type: http
- additional_required_headers:
  - description: Email of the end customer the call acts on. Required on every connection method; the SDK throws before sending if it is missing.
    name: x-user-email
  api: pabbly:pabbly-connect-platform
  format: Bearer pk_live_...
  header: Authorization
  id: connect-platform-bearer
  in: header
  key_prefix: pk_
  posture: Backend-to-backend only. The SDK states the tenant key and vended tokens must never reach a browser, a mobile app or an LLM context.
  scheme: bearer
  source: npm @pabbly/connect-platform@1.0.0 (index.js)
  type: http
slug: pabbly-authentication
source_filename: pabbly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://apidocs.pabbly.com/pabbly/subscription-billing/llms.txt\ndocs: https://apidocs.pabbly.com/\nprovider: Pabbly\nproviderId: pabbly\nsummary: >-\n  Pabbly uses per-product credentials generated from the account dashboard. Three\n  of the five documented REST APIs use HTTP Basic auth with an API Key as the\n  username and a Secret Key as the password; two use a Bearer token. The sixth\n  API — Connect Platform — uses a Bearer tenant key prefixed pk_live_ plus a\n  required x-user-email header naming the end customer the call acts on. No\n  OAuth 2.0, no OpenID Connect and no mTLS are published anywhere on the surface;\n  every /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n  probe returned 404.\nschemes:\n  - id: subscription-billing-basic\n    api: pabbly:pabbly-subscriptions\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    format: 'Basic <base64(API_KEY:SECRET_KEY)>'\n\
  \    credential_source: Pabbly dashboard -> Settings -> API Settings -> Generate the Keys\n    credentials:\n      - name: API Key\n        role: basic username\n      - name: Secret Key\n        role: basic password\n    rotation: Regenerate from Settings -> API Settings -> Generate the Keys\n    docs: https://apidocs.pabbly.com/subscription-billing/reference/guides/authentication\n  - id: hook-basic\n    api: pabbly:pabbly-hook\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    format: 'Basic <base64(API_KEY:SECRET_KEY)>'\n    credential_source: Pabbly dashboard -> Settings -> API Settings -> Generate the Keys\n    docs: https://apidocs.pabbly.com/hook/reference/guides/authentication\n  - id: email-verification-basic\n    api: pabbly:pabbly-email-verification\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    format: 'Basic <base64(API_KEY:SECRET_KEY)>'\n    credential_source: Pabbly dashboard -> Settings -> API -> Generate\
  \ API Keys\n    docs: https://apidocs.pabbly.com/email-verification/reference/guides/authentication\n  - id: chatflow-bearer\n    api: pabbly:pabbly-chatflow\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <API_KEY>'\n    credential_source: Pabbly Chatflow -> Settings -> API & Webhooks\n    credentials:\n      - name: API key\n        role: bearer token\n    docs: https://apidocs.pabbly.com/chatflow/reference/guides/authentication\n  - id: email-marketing-bearer\n    api: pabbly:pabbly-email-marketing\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <API_KEY>'\n    docs: https://apidocs.pabbly.com/email-marketing/reference/guides/authentication\n  - id: connect-platform-bearer\n    api: pabbly:pabbly-connect-platform\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer pk_live_...'\n    key_prefix: pk_\n    additional_required_headers:\n\
  \      - name: x-user-email\n        description: >-\n          Email of the end customer the call acts on. Required on every\n          connection method; the SDK throws before sending if it is missing.\n    posture: >-\n      Backend-to-backend only. The SDK states the tenant key and vended tokens\n      must never reach a browser, a mobile app or an LLM context.\n    source: npm @pabbly/connect-platform@1.0.0 (index.js)\nnot_supported:\n  - oauth2\n  - openIdConnect\n  - mutualTLS\n  - apiKey-in-query\n  - request-signing\nobservations:\n  - >-\n    Credentials are account-wide and unscoped — there is no permissions or scope\n    surface published for any Pabbly API, so a key grants whatever the account\n    can do. Pabbly's own docs say so: \"Your credentials grant full access to your\n    account.\"\n  - >-\n    Basic-auth products send the secret on every request rather than exchanging\n    it for a short-lived token; there is no documented expiry or refresh.\n  - >-\n    Auth differs\
  \ per product (Basic vs Bearer) with no shared identity layer,\n    so a multi-product integration carries several unrelated credentials.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pabbly/refs/heads/main/authentication/pabbly-authentication.yml
summary_line: 6 schemes
tags:
- Automation
- Email Marketing
- Subscription Billing
- Billing
- Payments
- Webhooks
- Messaging
- WhatsApp
- Email Verification
- Forms
- No-Code
- SaaS
---
