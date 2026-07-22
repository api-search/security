---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: notch.financial
  spf: true
hosts:
- cert_expires: Sep 18 02:22:49 2026 GMT
  host: www.notch.financial
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Notch
provider_slug: notch
slug: notch-domain-security
source_filename: notch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notch.financial\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notch.financial\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notch/refs/heads/main/security/notch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurant
- Foodservice
- Ordering
- Supply Chain
- Suppliers
- Distributors
- Accounts Payable
- Accounts Receivable
- Invoicing
- Payments
- Reconciliation
- ERP Integration
- Accounting
---
