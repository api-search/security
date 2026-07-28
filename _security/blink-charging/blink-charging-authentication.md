---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Blink Charging Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blink Charging declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Blink Charging
provider_slug: blink-charging
scheme_count: 0
schemes: []
slug: blink-charging-authentication
source_filename: blink-charging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://blinkcharging.com/legal/blink-network-terms-and-conditions,\n  https://github.com/blinkcharging/kong-oidc, and live probes of api.blinknetwork.com and\n  host.blinknetwork.com (2026-07-27).\ndocumented: false\npointer_withheld: true\npointer_withheld_reason: >-\n  No `Authentication` pointer was wired into apis.yml. The apis.io `authentication_documented`\n  check rewards a provider for PUBLISHING an auth contract, and Blink publishes none - no scheme\n  name, header, token format, flow, scope or credential-issuance path appears on any Blink\n  surface. Wiring the pointer would claim a documented auth surface that does not exist. This file\n  records what is knowable so the pointer can be added the day Blink documents it.\n\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  spec_derived: false\n  note: >-\n    derive-authentication.py was not run - there is no OpenAPI/Swagger in this repo to derive\n\
  \    securitySchemes from, by design (see review.yml harvest.explicitlyNotHarvested).\n\nevidence:\n- source: https://blinkcharging.com/legal/blink-network-terms-and-conditions\n  kind: terms-of-service\n  detail: >-\n    \"Last Modified: December 2, 2025.\" Section 8, \"Using the Blink Website, API, or Mobile\n    Applications\", states verbatim: \"You are responsible for all use of the Blink Website, API,\n    and Mobile Applications under your username.\" This is the only first-party statement about\n    Blink API authentication that exists: it implies username-scoped account credentials and\n    nothing more.\n- source: https://github.com/blinkcharging/kong-oidc\n  kind: inference\n  detail: >-\n    Blink's GitHub organisation maintains a single public repo - an Apache-2.0 fork of\n    S44-Automotive/kong-oidc (\"OIDC plugin for Kong\"), created 2024-06-17. The live gateway at\n    api.blinknetwork.com advertises `server: kong/2.8.1`. Together these suggest OIDC in front of\n    the\
  \ Kong gateway, but no OIDC discovery document is published (see below) and no client\n    registration path exists. Recorded as inference, NOT as a scheme.\n- source: https://api.blinknetwork.com/\n  kind: probe\n  detail: >-\n    Kong returns HTTP 404 {\"message\":\"no Route matched with those values\"} for unmatched paths;\n    /oauth/token and /auth are both unmatched. No 401 challenge, no WWW-Authenticate header and no\n    token endpoint is exposed anonymously.\n- source: https://host.blinknetwork.com/\n  kind: probe\n  detail: >-\n    The Blink Network host portal is a React SPA served from AmazonS3 behind CloudFront. Its login\n    is a human account login for hosts, not a documented API credential flow.\n- source: historical\n  kind: retired-surface\n  detail: >-\n    The retired BlinkMap API (prod.blinknetwork.com/developer.html, last archived 2021-07-28)\n    granted \"access to our technical documentation and email support\" only after an application\n    form and agreement\
  \ to the \"Blink Network, LLC Data License Agreement\" - i.e. even the auth\n    documentation was behind the approval gate.\n\ndiscovery_probes:\n- {url: 'https://blinkcharging.com/.well-known/openid-configuration', status: 404}\n- {url: 'https://blinkcharging.com/.well-known/oauth-authorization-server', status: 404}\n- {url: 'https://host.blinknetwork.com/.well-known/openid-configuration', status: '200 (soft - 959-byte React SPA shell, text/html)'}\n- {url: 'https://api.blinknetwork.com/.well-known/security.txt', status: '404 (Kong no-route)'}\n\naccess_gate:\n  gate: application-approval\n  self_serve: false\n  detail: >-\n    There is no self-serve credential path. The two live routes to any Blink data are (1) the UK\n    open data Google Form at https://blinkcharging.com/en-gb/getintouch/blink-open-data-request and\n    (2) \"contact support if you need access to OCPI\", the message Blink's own gateway returns on\n    /map/*.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blink-charging/refs/heads/main/authentication/blink-charging-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- United States
- EV Charging
- Electric Vehicles
- Charging Stations
- Grid
- Demand Response
- Fleet Management
- OCPP
- OpenADR
- Roaming
---
