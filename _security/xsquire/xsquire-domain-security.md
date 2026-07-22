---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xsquare.biz
  spf: true
hosts:
- cert_expires: Sep 18 02:41:16 2026 GMT
  host: xsquare.biz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xsquire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XSquare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XSquare
provider_slug: xsquire
slug: xsquire-domain-security
source_filename: xsquire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xsquare.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xsquare.biz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xsquire/refs/heads/main/security/xsquire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Invoicing
- Reconciliation
- B2B
- Accounts Payable
- Accounts Receivable
- E-Invoicing
- United Arab Emirates
- Qatar
---
