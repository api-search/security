---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: motorola.com
  spf: true
hosts:
- cert_expires: Oct  7 17:57:15 2026 GMT
  host: motorola.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motorola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motorola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Motorola
provider_slug: motorola
slug: motorola-domain-security
source_filename: motorola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motorola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:57:15 2026 GMT\n  hsts: null\ndomains:\n- domain: motorola.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motorola/refs/heads/main/security/motorola-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer Electronics
- Smartphones
- Mobile Devices
- Android
- Hardware
- Lenovo
---
