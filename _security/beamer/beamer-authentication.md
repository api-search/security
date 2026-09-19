---
anonymous_access: false
api_key_in: []
auth_types: []
description: Beamer's REST API authenticates with a single account-scoped API key sent in a custom header. There is no OAuth, no OpenID Connect, no mTLS and no scope surface — a key carries every permission the account has, including destructive team and privacy operations.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Beamer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beamer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Beamer
provider_slug: beamer
scheme_count: 2
schemes:
- description: Account API key, retrieved from the Beamer dashboard under Settings > API (https://app.getbeamer.com/settings#api). Required on every request; the reference documents a 401 "Either no API key was provided or the provided API key is invalid" on all 49 operations.
  id: Beamer-Api-Key
  in: header
  name: Beamer-Api-Key
  rotation: not documented
  scopes: []
  type: apiKey
- description: Shared secret Beamer sends on every outbound webhook POST so the receiver can validate authenticity. Auto-generated per webhook and readable in the dashboard. It is a static shared secret, not a signature (no HMAC over the body, no timestamp, no replay window).
  direction: inbound
  id: Beamer-Webhook-Secret
  in: header
  name: Beamer-Webhook-Secret
  source: https://help.userflow.com/beamer/docs/developer-documentation
  type: apiKey
slug: beamer-authentication
source_filename: beamer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://getbeamer-api.pages.dev/\ndocs: https://getbeamer-api.pages.dev/\ndescription: >-\n  Beamer's REST API authenticates with a single account-scoped API key sent in a custom header. There\n  is no OAuth, no OpenID Connect, no mTLS and no scope surface — a key carries every permission the\n  account has, including destructive team and privacy operations.\napi_base: https://api.getbeamer.com/v0\nschemes:\n  - id: Beamer-Api-Key\n    type: apiKey\n    in: header\n    name: Beamer-Api-Key\n    description: >-\n      Account API key, retrieved from the Beamer dashboard under Settings > API\n      (https://app.getbeamer.com/settings#api). Required on every request; the reference documents a\n      401 \"Either no API key was provided or the provided API key is invalid\" on all 49 operations.\n    scopes: []\n    rotation: not documented\n  - id: Beamer-Webhook-Secret\n    type: apiKey\n    in: header\n    name: Beamer-Webhook-Secret\n\
  \    direction: inbound\n    description: >-\n      Shared secret Beamer sends on every outbound webhook POST so the receiver can validate\n      authenticity. Auto-generated per webhook and readable in the dashboard. It is a static shared\n      secret, not a signature (no HMAC over the body, no timestamp, no replay window).\n    source: https://help.userflow.com/beamer/docs/developer-documentation\nobserved:\n  - url: https://api.getbeamer.com/v0/url\n    method: GET\n    sent_credentials: none\n    http_status: 401\n    content_type: application/json;charset=utf-8\n    body: '\"The API key is invalid.\"'\n    note: probed 2026-09-14 — unauthenticated requests are rejected, confirming the scheme is enforced.\noauth: false\nopenid_connect: false\nmtls: false\nscopes_documented: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beamer/refs/heads/main/authentication/beamer-authentication.yml
summary_line: 2 schemes
tags:
- Changelog
- Deprecation
- Notification
- Product Updates
- User Engagement
- Webhook
- NPS
- Feedback
---
