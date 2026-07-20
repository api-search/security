---
api_specs:
- filename: daily-openapi-original.json
  format: json
  label: Daily API
  slug: daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/openapi/daily-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:help@daily.co"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daily.co
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.daily.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Daily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daily
provider_slug: daily
slug: daily-domain-security
source_filename: daily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.daily.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: daily.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:help@daily.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daily/refs/heads/main/security/daily-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Video
- Audio
- WebRTC
- Real-Time Communication
- Video Conferencing
- Live Streaming
- Recording
- Transcription
- Telephony
- SIP
- PSTN
- Company
---
