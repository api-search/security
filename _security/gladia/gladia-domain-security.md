---
api_specs:
- filename: api-reference
  format: yaml
  label: Gladia Pre-recorded (Async) API
  slug: gladia-pre-recorded-async-api
  spec_type: OpenAPI
  url: https://docs.gladia.io/api-reference
- filename: docs
  format: yaml
  label: Gladia Live (Real-time) API
  slug: gladia-live-real-time-api
  spec_type: AsyncAPI
  url: https://github.com/gladiaio/docs
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gladia.io
  spf: true
hosts:
- cert_expires: Aug 15 21:23:50 2026 GMT
  host: www.gladia.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:44:12 2026 GMT
  host: docs.gladia.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 11:02:37 2026 GMT
  host: api.gladia.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gladia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gladia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gladia
provider_slug: gladia
slug: gladia-domain-security
source_filename: gladia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gladia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.gladia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:44:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gladia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:02:37 2026 GMT\n  hsts: null\ndomains:\n- domain: gladia.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gladia/refs/heads/main/security/gladia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Speech-to-Text
- Transcription
- Audio Intelligence
- Real-Time
- Speaker Diarization
- Translation
- WebSocket
- REST
---
