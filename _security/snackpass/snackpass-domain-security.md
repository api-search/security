---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snackpass.co
  spf: true
hosts:
- cert_expires: Oct  7 12:16:10 2026 GMT
  host: web.snackpass.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snackpass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snackpass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Snackpass
provider_slug: snackpass
slug: snackpass-domain-security
source_filename: snackpass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.snackpass.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snackpass.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snackpass/refs/heads/main/security/snackpass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurants
- Point of Sale
- Payments
- Food Ordering
- Loyalty
- Marketing
- Kiosk
- Hospitality
---
