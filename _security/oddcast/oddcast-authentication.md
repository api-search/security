---
api_key_in:
- query
auth_types:
- apiKey
- checksum
description: ''
kind: authentication
layout: security
method: searched
name: Oddcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oddcast secures its APIs with apiKey and checksum across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oddcast
provider_slug: oddcast
scheme_count: 2
schemes:
- docs: https://www.vocalware.com/support/reference
  in: query
  mechanism: Account id (ACC) and API key are issued from the Vocalware account. Each HTTP/REST or JavaScript request carries the account id and a checksum (CS) derived from the request parameters and the secret API key; the secret key itself is not transmitted on the request. Requests are metered per audio stream (one playback instance up to 60 seconds).
  name: VocalwareRequestSignature
  product: Vocalware Text-to-Speech API
  sources:
  - searched:https://www.vocalware.com/support/reference
  type: apiKey
- docs: https://www.sitepal.com/guide
  in: embed
  login: https://vhost.oddcast.com/admin/index.php
  mechanism: A SitePal scene is bound to an account id and embedded via the SitePal JavaScript (VHost) API; runtime control (sayText, sayAI, etc.) executes in the browser under that account. Account/admin access is via the VHost login.
  name: SitePalAccount
  product: SitePal Avatar API
  sources:
  - searched:https://www.sitepal.com/guide
  type: apiKey
slug: oddcast-authentication
source_filename: oddcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.vocalware.com/support/reference\ndocs: https://www.vocalware.com/support/reference\nsummary:\n  types: [apiKey, checksum]\n  api_key_in: [query]\n  notes: >-\n    Oddcast's developer products do not use OAuth. Vocalware authenticates each\n    text-to-speech request with an account identifier plus a secret API key and a\n    per-request checksum (signature) computed over the request parameters, so the\n    secret key is never sent in the clear. SitePal avatars are provisioned to an\n    account and embedded/controlled client-side; server-side account access is via\n    the VHost admin login.\nschemes:\n- name: VocalwareRequestSignature\n  product: Vocalware Text-to-Speech API\n  type: apiKey\n  in: query\n  mechanism: >-\n    Account id (ACC) and API key are issued from the Vocalware account. Each\n    HTTP/REST or JavaScript request carries the account id and a checksum (CS)\n    derived from the request parameters\
  \ and the secret API key; the secret key\n    itself is not transmitted on the request. Requests are metered per audio\n    stream (one playback instance up to 60 seconds).\n  docs: https://www.vocalware.com/support/reference\n  sources: [searched:https://www.vocalware.com/support/reference]\n- name: SitePalAccount\n  product: SitePal Avatar API\n  type: apiKey\n  in: embed\n  mechanism: >-\n    A SitePal scene is bound to an account id and embedded via the SitePal\n    JavaScript (VHost) API; runtime control (sayText, sayAI, etc.) executes in the\n    browser under that account. Account/admin access is via the VHost login.\n  docs: https://www.sitepal.com/guide\n  login: https://vhost.oddcast.com/admin/index.php\n  sources: [searched:https://www.sitepal.com/guide]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddcast/refs/heads/main/authentication/oddcast-authentication.yml
summary_line: apiKey/checksum · 2 schemes
tags:
- Company
- Text-to-Speech
- Speech Synthesis
- Avatars
- Voice
- Media
- Creative Technology
- Education
- Developers
---
