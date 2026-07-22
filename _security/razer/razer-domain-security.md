---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: razer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: razerzone.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: razer.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: assets.razerzone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: chromasdk.io
  https: false
kind: domain-security
layout: security
method: probed
name: Razer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Razer, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Razer
provider_slug: razer
slug: razer-domain-security
source_filename: razer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: razer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: assets.razerzone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\n- host: chromasdk.io\n  https: false\ndomains:\n- domain: razer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: razerzone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razer/refs/heads/main/security/razer-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Gaming
- Hardware
- Peripherals
- RGB Lighting
- Haptics
- Payments
- Developer Platform
- SDK
---
