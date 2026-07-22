---
api_key_in: []
auth_types:
- none
- custom-credentials
- user-sign-in
description: ''
kind: authentication
layout: security
method: searched
name: Razer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Razer secures its APIs with none, custom-credentials, and user-sign-in across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Razer
provider_slug: razer
scheme_count: 3
schemes:
- description: Razer ID is Razer's user identity / single sign-on service. Developers integrate it to authenticate and onboard verified Razer users across mobile and web via per-platform SDK guides (Android/iOS/Web).
  docs: https://developer.razer.com/razerid
  name: Razer ID Sign-In
  program: razerid
  type: user-sign-in
- description: The Razer Gold payment API authenticates approved merchants/partners with issued merchant credentials; full auth/signature details are provided in the partner documentation at https://api.razer.com/docs.
  docs: https://developer.razer.com/razer-gold-developer-and-partner-program
  name: Razer Gold merchant credentials
  program: razer-gold
  type: custom-credentials
- description: The Chroma REST API runs on the local machine (localhost:54235) alongside Razer Synapse; no API key or bearer token is required — access is scoped to the local session URI.
  docs: https://assets.razerzone.com/dev_portal/REST/html/index.html
  name: Razer Chroma REST (local)
  program: chroma
  type: none
slug: razer-authentication
source_filename: razer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.razer.com/ (Razer ID, Razer Gold, Chroma developer programs)\nnotes: >-\n  Razer does not publish a single OpenAPI securityScheme surface; auth differs per\n  program. Captured from the developer portal at a high level (no spec to derive\n  from). Detailed OAuth endpoints/scopes for Razer ID and merchant credentials for\n  Razer Gold are published in per-platform PDF guides behind the developer portal.\nsummary:\n  types:\n  - none\n  - custom-credentials\n  - user-sign-in\nschemes:\n- name: Razer ID Sign-In\n  program: razerid\n  type: user-sign-in\n  docs: https://developer.razer.com/razerid\n  description: >-\n    Razer ID is Razer's user identity / single sign-on service. Developers integrate\n    it to authenticate and onboard verified Razer users across mobile and web via\n    per-platform SDK guides (Android/iOS/Web).\n- name: Razer Gold merchant credentials\n  program: razer-gold\n  type: custom-credentials\n\
  \  docs: https://developer.razer.com/razer-gold-developer-and-partner-program\n  description: >-\n    The Razer Gold payment API authenticates approved merchants/partners with\n    issued merchant credentials; full auth/signature details are provided in the\n    partner documentation at https://api.razer.com/docs.\n- name: Razer Chroma REST (local)\n  program: chroma\n  type: none\n  docs: https://assets.razerzone.com/dev_portal/REST/html/index.html\n  description: >-\n    The Chroma REST API runs on the local machine (localhost:54235) alongside\n    Razer Synapse; no API key or bearer token is required — access is scoped to\n    the local session URI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razer/refs/heads/main/authentication/razer-authentication.yml
summary_line: none/custom-credentials/user-sign-in · 3 schemes
tags:
- Company
- Consumer
- Gaming
- Hardware
- Peripherals
- RGB Lighting
- Haptics
- Payments
- Developer Platform
- SDK
---
