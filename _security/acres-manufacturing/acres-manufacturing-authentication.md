---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Acres Manufacturing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acres Manufacturing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Acres Manufacturing
provider_slug: acres-manufacturing
scheme_count: 1
schemes:
- described_in: provider FAQ
  described_in_contract: false
  evidence: '"APIs require mTLS for authentication" — https://acresmanufacturing.com/faq/'
  in: transport
  name: Client certificate (mTLS)
  note: The mechanism is asserted on the marketing FAQ, not in the API reference. Certificate issuance, rotation, revocation and the trust anchor are undocumented publicly.
  type: mutualTLS
slug: acres-manufacturing-authentication
source_filename: acres-manufacturing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://acresmanufacturing.com/faq/ (\"Is Foundation secure? All Foundation network communication\n  utilizes the latest encryption standards (TLS 1.3). Furthermore, APIs require mTLS for\n  authentication.\") and\n  https://github.com/acres4/foundation-documentation/blob/master/apis/event/1.4/usage.md\ndocs: https://acresmanufacturing.com/faq/\nsummary: >-\n  Acres states publicly that Foundation APIs authenticate with mutual TLS. The Foundation Event\n  Replay API reference itself documents no credential, header, token or handshake — it shows only\n  the WebSocket URL and its query filters — so a partner obtains and installs a client certificate\n  through the casino property and Acres, not through a self-service developer portal. There is no\n  OAuth, no OpenID Connect, no API key and no published key-issuance flow.\nschemes:\n- type: mutualTLS\n  name: Client certificate (mTLS)\n  in: transport\n  described_in: provider\
  \ FAQ\n  described_in_contract: false\n  evidence: >-\n    \"APIs require mTLS for authentication\" — https://acresmanufacturing.com/faq/\n  note: >-\n    The mechanism is asserted on the marketing FAQ, not in the API reference. Certificate issuance,\n    rotation, revocation and the trust anchor are undocumented publicly.\ntransport_security:\n  tls: 'TLS 1.3'\n  evidence: https://acresmanufacturing.com/faq/\noauth2: false\nopenid_connect: false\napi_key: false\nbasic_auth: false\nscopes_published: false\nself_service_signup: false\nonboarding: >-\n  Access is granted per property. The consumer connects to their own casino's Foundation host\n  (wss://{property}.kailabor.com), which implies the operator provisions the partner rather than\n  Acres issuing public credentials.\ngaps:\n- The API reference documents no authentication at all; the only statement is on the FAQ page.\n- No certificate-issuance, rotation or revocation procedure is published.\n- No documented error response for an\
  \ authentication failure (the only documented error is HTTP 400 on a non-upgraded request).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acres-manufacturing/refs/heads/main/authentication/acres-manufacturing-authentication.yml
summary_line: 1 scheme
tags:
- Casino Gaming
- Casino Management System
- Gaming Technology
- Slot Machines
- Cashless Payments
- Real-Time Data
- Event Streaming
- WebSocket
- Bluetooth Low Energy
- Loyalty and Bonusing
- Hospitality
---
