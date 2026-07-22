---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: artiphon.com
  spf: true
hosts:
- cert_expires: Oct 10 15:45:43 2026 GMT
  host: artiphon.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artiphon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artiphon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Artiphon
provider_slug: artiphon
slug: artiphon-domain-security
source_filename: artiphon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artiphon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:45:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: artiphon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artiphon/refs/heads/main/security/artiphon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Music
- Musical Instruments
- MIDI
- Hardware
- Consumer Electronics
- Audio
- Synthesizer
---
