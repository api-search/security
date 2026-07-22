---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jupiter.money
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: jupiter.money
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupiter Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupiter Money, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Jupiter Money
provider_slug: jupiter-money
slug: jupiter-money-domain-security
source_filename: jupiter-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupiter.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: jupiter.money\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiter-money/refs/heads/main/security/jupiter-money-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Banking
- Neobank
- Digital Banking
- Fintech
- Consumer Finance
- Personal Finance
- Savings
- Lending
- Credit Cards
- UPI
- Payments
- Mutual Funds
- Digital Gold
- Rewards
- India
---
