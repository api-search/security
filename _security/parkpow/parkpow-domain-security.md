---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parkpow.com
  spf: true
hosts:
- cert_expires: Aug 11 21:55:56 2026 GMT
  host: parkpow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 12:42:58 2026 GMT
  host: app.parkpow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parkpow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParkPow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ParkPow
provider_slug: parkpow
slug: parkpow-domain-security
source_filename: parkpow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parkpow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 21:55:56 2026 GMT\n  hsts: false\n- host: app.parkpow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:42:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parkpow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parkpow/refs/heads/main/security/parkpow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parking
- License Plate Recognition
- Enforcement
---
