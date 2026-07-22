---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trycents.com
  spf: true
hosts:
- cert_expires: Sep 21 23:46:32 2026 GMT
  host: www.trycents.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cents
provider_slug: cents
slug: cents-domain-security
source_filename: cents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trycents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trycents.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cents/refs/heads/main/security/cents-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- Laundry
- Point of Sale
- Payments
- Business Management
- Pickup and Delivery
- SaaS
- Small Business
---
