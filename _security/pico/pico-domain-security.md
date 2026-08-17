---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hype.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trypico.com
  spf: true
hosts:
- cert_expires: Sep 28 21:07:24 2026 GMT
  host: www.hype.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 19:46:16 2026 GMT
  host: docs.trypico.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.trypico.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pico, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pico
provider_slug: pico
slug: pico-domain-security
source_filename: pico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hype.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trypico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 19:46:16 2026 GMT\n  hsts: null\n- host: api.trypico.com\n  https: false\ndomains:\n- domain: hype.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: trypico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico/refs/heads/main/security/pico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- CRM
- Memberships
- Payments
- Email Marketing
- Newsletters
- Monetization
- Retired
---
