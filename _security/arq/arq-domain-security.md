---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arqfinance.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.arqfinance.com
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arq
provider_slug: arq
slug: arq-domain-security
source_filename: arq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arqfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400000\ndomains:\n- domain: arqfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arq/refs/heads/main/security/arq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Payments
- Cross-Border Payments
- Stablecoin
- Digital Wallet
- Banking
- Investing
- Latin America
- Mexico
---
