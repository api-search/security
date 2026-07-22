---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alphaventuredao.io
  spf: true
hosts:
- cert_expires: Oct  3 20:33:05 2026 GMT
  host: alphaventuredao.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpha Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpha Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alpha Finance
provider_slug: alpha-finance
slug: alpha-finance-domain-security
source_filename: alpha-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphaventuredao.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:33:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alphaventuredao.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-finance/refs/heads/main/security/alpha-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- Blockchain
- Smart Contracts
- Yield Farming
- DAO
- Lending
---
