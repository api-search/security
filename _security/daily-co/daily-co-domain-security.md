---
api_specs:
- filename: daily-co-openapi.yml
  format: yaml
  label: Daily REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily-co/refs/heads/main/openapi/daily-co-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daily.co
  spf: true
hosts:
- cert_expires: Sep 22 13:48:52 2026 GMT
  host: www.daily.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 18:03:59 2026 GMT
  host: docs.daily.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.daily.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Daily Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daily, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daily
provider_slug: daily-co
slug: daily-co-domain-security
source_filename: daily-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daily.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:48:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.daily.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:03:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.daily.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: daily.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily-co/refs/heads/main/security/daily-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Realtime
- WebRTC
- Video
- Audio
- SDK
- Voice AI
- Recording
- Transcription
---
