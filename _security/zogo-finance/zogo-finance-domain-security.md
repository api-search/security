---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zogofinance.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: zogofinance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zogo Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zogo Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zogo Finance
provider_slug: zogo-finance
slug: zogo-finance-domain-security
source_filename: zogo-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zogofinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zogofinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zogo-finance/refs/heads/main/security/zogo-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Literacy
- Financial Education
- FinTech
- Gamification
- Banking
- Credit Unions
- SDK
- EdTech
---
