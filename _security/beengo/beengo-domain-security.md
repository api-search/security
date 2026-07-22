---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appfront.ai
  spf: true
hosts:
- cert_expires: Aug 19 21:32:37 2026 GMT
  host: appfront.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beengo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beengo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beengo
provider_slug: beengo
slug: beengo-domain-security
source_filename: beengo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appfront.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:32:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appfront.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beengo/refs/heads/main/security/beengo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurant
- Restaurant Engagement
- Online Ordering
- Loyalty
- Point of Sale
- Food Service
- eCommerce
- Marketing
- Payments
---
