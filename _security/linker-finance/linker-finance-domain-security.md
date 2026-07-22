---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linkerfinance.com
  spf: true
hosts:
- cert_expires: Sep 29 07:44:10 2026 GMT
  host: linkerfinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linker Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linker Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linker Finance
provider_slug: linker-finance
slug: linker-finance-domain-security
source_filename: linker-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkerfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linkerfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linker-finance/refs/heads/main/security/linker-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Banking
- Digital Banking
- Community Banking
- Commercial Banking
- Account Opening
- Onboarding
- KYC
- KYB
- AML
- Fraud Prevention
- Treasury Management
- CRM
- Fintech
- SaaS
---
