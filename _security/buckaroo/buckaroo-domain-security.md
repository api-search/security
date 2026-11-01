---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: buckaroo.eu
  spf: true
hosts:
- cert_expires: Dec 28 11:52:24 2026 GMT
  host: buckaroo.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buckaroo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buckaroo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Buckaroo
provider_slug: buckaroo
slug: buckaroo-domain-security
source_filename: buckaroo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buckaroo.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buckaroo.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buckaroo/security/buckaroo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Online Payments
- In‑store Payments
- Omnichannel
- Credit Management
- Subscription Management
- Business Lending
- Payment Terminals
---
