---
api_specs:
- filename: partykit-asyncapi.yml
  format: yaml
  label: PartyKit Deployed Party (HTTP / WebSocket)
  slug: deployed-party-http
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/partykit/refs/heads/main/asyncapi/partykit-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: partykit.io
  spf: true
hosts:
- cert_expires: Sep  5 12:07:11 2026 GMT
  host: www.partykit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:22:31 2026 GMT
  host: docs.partykit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partykit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PartyKit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PartyKit
provider_slug: partykit
slug: partykit-domain-security
source_filename: partykit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.partykit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:07:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.partykit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: partykit.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partykit/refs/heads/main/security/partykit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Real-Time
- Multiplayer
- WebSockets
- Cloudflare
- Durable Objects
- Edge
- CRDT
- Yjs
- Serverless
---
