---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jinglepay.com
  spf: true
hosts:
- cert_expires: Sep 25 19:29:49 2026 GMT
  host: jinglepay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jingle Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jingle Pay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jingle Pay
provider_slug: jingle-pay
slug: jingle-pay-domain-security
source_filename: jingle-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jinglepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:29:49 2026 GMT\n  hsts: false\ndomains:\n- domain: jinglepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jingle-pay/refs/heads/main/security/jingle-pay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Digital Wallet
- Financial Services
- MENA
---
