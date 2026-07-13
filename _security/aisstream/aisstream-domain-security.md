---
api_specs:
- filename: aisstream-asyncapi.yml
  format: yaml
  label: AISStream AIS Stream API
  slug: aisstream-ais-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aisstream/refs/heads/main/asyncapi/aisstream-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aisstream.io
  spf: true
hosts:
- cert_expires: Aug 26 03:21:49 2026 GMT
  host: aisstream.io
  hsts: false
  http_status: 403
  https: true
  notes: Homepage/docs sit behind Cloudflare (managed challenge to bots); returns 403 to non-browser clients.
  tls_version: TLSv1.3
- cert_expires: Jul 19 22:34:56 2026 GMT
  host: stream.aisstream.io
  hsts: false
  http_status: 404
  https: true
  notes: WebSocket endpoint host (wss://stream.aisstream.io/v0/stream). A plain HTTPS GET returns 404; the socket is reached via the WebSocket upgrade.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aisstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AISStream, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AISStream
provider_slug: aisstream
slug: aisstream-domain-security
source_filename: aisstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + WebSocket hosts\nhosts:\n- host: aisstream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:21:49 2026 GMT\n  hsts: false\n  http_status: 403\n  notes: Homepage/docs sit behind Cloudflare (managed challenge to bots); returns 403 to non-browser clients.\n- host: stream.aisstream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 19 22:34:56 2026 GMT\n  hsts: false\n  http_status: 404\n  notes: WebSocket endpoint host (wss://stream.aisstream.io/v0/stream). A plain HTTPS GET returns 404; the socket is reached via the WebSocket upgrade.\ndomains:\n- domain: aisstream.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisstream/refs/heads/main/security/aisstream-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vessel Tracking
- AIS
- Maritime
- Ship Tracking
- Real-Time Data
- WebSocket
- Streaming
- Ships
- Maritime Data
- Location
---
