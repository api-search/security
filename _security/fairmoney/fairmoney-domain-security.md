---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fairmoney.io
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: fairmoney.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fairmoney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FairMoney, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FairMoney
provider_slug: fairmoney
slug: fairmoney-domain-security
source_filename: fairmoney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairmoney.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fairmoney.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairmoney/refs/heads/main/security/fairmoney-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Digital Bank
- Neobank
- Mobile Banking
- Micro-Lending
- Consumer Credit
- Personal Loans
- Savings
- Cards
- Payments
- Business Banking
- SME Banking
- Financial Inclusion
- Emerging Markets
- Nigeria
- India
- Africa
- Fintech
---
