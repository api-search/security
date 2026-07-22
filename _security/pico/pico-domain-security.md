---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trypico.com
  spf: true
hosts:
- cert_expires: Aug 26 20:02:33 2026 GMT
  host: trypico.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:02:33 2026 GMT
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
overview: 'Domain security posture for Pico, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pico
provider_slug: pico
slug: pico-domain-security
source_filename: pico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trypico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:02:33 2026 GMT\n  hsts: null\n- host: docs.trypico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:02:33 2026 GMT\n  hsts: null\n- host: api.trypico.com\n  https: false\ndomains:\n- domain: trypico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pico/refs/heads/main/security/pico-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Creator Economy
- CRM
- Memberships
- Payments
- Email Marketing
- Newsletters
- Monetization
---
