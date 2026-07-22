---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: saffron.finance
  spf: false
hosts:
- cert_expires: Sep 16 11:43:47 2026 GMT
  host: saffron.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saffron Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saffron Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Saffron Finance
provider_slug: saffron-finance
slug: saffron-finance-domain-security
source_filename: saffron-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saffron.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: saffron.finance\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saffron-finance/refs/heads/main/security/saffron-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Web3
- DeFi
- Yield
- Fixed Income
- Vaults
- Ethereum
- Smart Contracts
- Governance
---
