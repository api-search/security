---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kiosk.app
  spf: false
hosts:
- cert_expires: Aug 19 05:20:18 2026 GMT
  host: kiosk.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiosk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiosk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kiosk
provider_slug: kiosk
slug: kiosk-domain-security
source_filename: kiosk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kiosk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kiosk.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiosk/refs/heads/main/security/kiosk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto
---
