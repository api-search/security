---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haulpay.io
  spf: true
hosts:
- cert_expires: Dec 24 16:40:40 2026 GMT
  host: haulpay.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HaulPay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HaulPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HaulPay
provider_slug: haulpay
slug: haulpay-domain-security
source_filename: haulpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haulpay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 16:40:40 2026 GMT\n  hsts: false\ndomains:\n- domain: haulpay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/haulpay/security/haulpay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Freight
- Finance
- Payments
- Logistics
---
