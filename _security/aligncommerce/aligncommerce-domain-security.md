---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alignecommerce.com
  spf: true
hosts:
- cert_expires: Dec  9 00:16:04 2026 GMT
  host: www.alignecommerce.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aligncommerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aligncommerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aligncommerce
provider_slug: aligncommerce
slug: aligncommerce-domain-security
source_filename: aligncommerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alignecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 00:16:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: alignecommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aligncommerce/refs/heads/main/security/aligncommerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- High‑Risk Merchants
- Chargeback Management
- Fraud Prevention
- E‑commerce Integration
---
