---
api_specs:
- filename: reactor-helios-asyncapi.yml
  format: yaml
  label: Reactor Realtime Video API
  slug: reactor-realtime-video-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/reactor/refs/heads/main/asyncapi/reactor-helios-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reactor.inc
  spf: true
hosts:
- cert_expires: Sep 21 05:46:52 2026 GMT
  host: reactor.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reactor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reactor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reactor
provider_slug: reactor
slug: reactor-domain-security
source_filename: reactor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reactor.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: reactor.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reactor/refs/heads/main/security/reactor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Video
- Generative AI
- Real-Time
- WebRTC
- Streaming
- SDK
- Media
---
