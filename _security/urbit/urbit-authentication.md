---
api_key_in: []
auth_types:
- cookie-session
description: 'Authentication profile for the Urbit ship HTTP API (Eyre, the Arvo HTTP server vane). There is no central Urbit API and no OAuth: every ship is a self-hosted personal server that authenticates web clients with a session cookie. The client obtains the ship''s web login code with +code in the dojo, POSTs it to /~/login, and receives an urbauth-~ship session cookie (observed Max-Age 604800 = 7 days) that must accompany all channel, scry, and thread requests. EAuth extends this with cross-ship web login (using one''s own ship as the identity provider on another ship''s site). The Azimuth PKI on Ethereum anchors identity keys; Bridge (bridge.urbit.org) manages them.'
kind: authentication
layout: security
method: searched
name: Urbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urbit secures its APIs with cookie-session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Urbit
provider_slug: urbit
scheme_count: 2
schemes:
- cookie_name: urbauth-~<ship>
  credential_source: +code (dojo web login code)
  description: 'POST password=<web-login-code> (from +code in the dojo) to /~/login; Eyre responds with set-cookie: urbauth-~<ship>=<token>; Path=/; Max-Age=604800. Include the cookie header on all subsequent requests. Invalid or missing cookies get 403 Forbidden.'
  docs: https://docs.urbit.org/urbit-os/kernel/eyre/external-api-ref#authentication
  login_path: /~/login
  name: eyre-session-cookie
  type: cookie
- description: 'EAuth: Eyre''s cross-ship authentication lets a user log into another ship''s web interface using their own ship as identity provider.'
  docs: https://docs.urbit.org/urbit-os/kernel/eyre/eauth
  name: eauth
  type: cross-ship-sso
slug: urbit-authentication
source_filename: urbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.urbit.org/urbit-os/kernel/eyre/external-api-ref.md\ndocs: https://docs.urbit.org/urbit-os/kernel/eyre/external-api-ref#authentication\ndescription: >-\n  Authentication profile for the Urbit ship HTTP API (Eyre, the Arvo HTTP\n  server vane). There is no central Urbit API and no OAuth: every ship is a\n  self-hosted personal server that authenticates web clients with a session\n  cookie. The client obtains the ship's web login code with +code in the dojo,\n  POSTs it to /~/login, and receives an urbauth-~ship session cookie\n  (observed Max-Age 604800 = 7 days) that must accompany all channel, scry,\n  and thread requests. EAuth extends this with cross-ship web login (using\n  one's own ship as the identity provider on another ship's site). The\n  Azimuth PKI on Ethereum anchors identity keys; Bridge (bridge.urbit.org)\n  manages them.\nsummary:\n  types: [cookie-session]\n  central_authority: none (per-ship, self-hosted)\n\
  \  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: eyre-session-cookie\n    type: cookie\n    description: >-\n      POST password=<web-login-code> (from +code in the dojo) to /~/login;\n      Eyre responds with set-cookie: urbauth-~<ship>=<token>; Path=/;\n      Max-Age=604800. Include the cookie header on all subsequent requests.\n      Invalid or missing cookies get 403 Forbidden.\n    login_path: /~/login\n    cookie_name: \"urbauth-~<ship>\"\n    credential_source: +code (dojo web login code)\n    docs: https://docs.urbit.org/urbit-os/kernel/eyre/external-api-ref#authentication\n  - name: eauth\n    type: cross-ship-sso\n    description: >-\n      EAuth: Eyre's cross-ship authentication lets a user log into another\n      ship's web interface using their own ship as identity provider.\n    docs: https://docs.urbit.org/urbit-os/kernel/eyre/eauth\nidentity_layer:\n  name: Azimuth (Urbit ID)\n  description: >-\n    Ethereum-anchored PKI: galaxies, stars, planets, moons, comets.\
  \ Networking\n    keys are set on-chain (L1) or via the Layer 2 naive rollup; Bridge is the\n    key-management client.\n  bridge: https://bridge.urbit.org/\n  docs: https://docs.urbit.org/urbit-id\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbit/refs/heads/main/authentication/urbit-authentication.yml
summary_line: cookie-session · 2 schemes
tags:
- Company
- Crypto
- Personal Servers
- Decentralized Identity
- Peer-to-Peer
- Operating Systems
- Self-Hosting
- Agents
---
