---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tapad Authentication
name_suffix: Authentication
oauth_flows: []
overview: TapAd declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TapAd
provider_slug: tapad
scheme_count: 0
schemes: []
slug: tapad-authentication
source_filename: tapad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://github.com/Tapad/tapestry-ios-sdk (README + TATapestryRequest.m) and\n  https://github.com/Tapad/tapestry-android-sdk — Tapad's own MIT-licensed SDK\n  source; corroborated by live unauthenticated probes of\n  https://tapestry.tapad.com/tapestry/1 on 2026-08-12.\nnote: >-\n  derive-authentication.py could not be run against a spec: Tapad publishes no\n  OpenAPI, so there are no securitySchemes to derive from. This profile is read\n  from Tapad's own published SDK source and confirmed against the live\n  endpoint. There is NO OAuth, NO bearer token, NO signed request and NO\n  Authorization header anywhere in Tapad's published surface — authentication is\n  a single partner identifier carried in the query string over TLS, plus an\n  origin/referrer check enforced server-side.\napis:\n\n  - api: tapestry\n    base_url: https://tapestry.tapad.com/tapestry/1\n    transport: HTTPS GET (query string); HSTS max-age=31536000\
  \ present on the response\n    schemes:\n      - id: partner_id\n        type: apiKey\n        in: query\n        name: ta_partner_id\n        required: true\n        description: >-\n          Partner identifier issued by Tapad. Configured in the iOS SDK as the\n          Info.plist key TapestryPartnerID and in the Android SDK via the\n          TapestryClient constructor. Absent or unrecognized values return\n          {\"errors\":[\"3|NoPartnerIdError\"]} with HTTP 200.\n        provisioning: manual, by Tapad (no self-service signup exists)\n        rotation: not documented\n      - id: referrer\n        type: origin-check\n        in: header\n        name: Referer\n        required: false\n        description: >-\n          The API validates the request referrer against the origin registered\n          for the partner id; a mismatch returns error 2|BadReferrerError. This\n          is a server-side control, not a credential the client chooses.\n    device_identity_parameters:\n   \
  \   - ta_partner_did\n      - ta_typed_did\n      - ta_partner_user_id\n    evidence:\n      - url: https://tapestry.tapad.com/tapestry/1\n        http_status: 200\n        body: '{\"errors\":[\"3|NoPartnerIdError\"]}'\n        fetched: '2026-08-12'\n      - url: https://tapestry.tapad.com/tapestry/1?ta_partner_id=1234&ta_get=\n        http_status: 200\n        body: '{\"errors\":[\"3|NoPartnerIdError\"]}'\n        fetched: '2026-08-12'\n        note: >-\n          A syntactically valid but unprovisioned partner id is rejected\n          identically — proof that partner ids are allocated, not self-asserted.\n\n  - api: event-tracking\n    base_url: https://analytics.tapad.com/app/event\n    transport: HTTPS GET beacon; responds 200 image/png (1x1 tracking pixel)\n    schemes:\n      - id: partner_id\n        type: apiKey\n        in: query\n        name: ta_partner_id\n        required: true\n        description: >-\n          Same partner identifier as the Tapestry API. Declared in\n\
  \          com.tapad.tracking.EventResource in the Android SDK.\n        provisioning: manual, by Tapad\n    evidence:\n      - url: https://analytics.tapad.com/app/event\n        http_status: 200\n        content_type: image/png\n        fetched: '2026-08-12'\n\noauth: false\nopenid_connect: false\nmutual_tls: false\ndocs: null\ndocs_note: >-\n  No public authentication documentation is served. docs.tapad.com 301s to\n  https://www.experian.com/marketing-knowledge-base/resolution, which states\n  \"This content is intended for Experian clients only.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapad/refs/heads/main/authentication/tapad-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- AdTech
- Identity
- Cross-Device
- Device Graph
- Marketing
- Data
- Attribution
- Audience
- Identity Resolution
---
