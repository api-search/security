---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cozy.finance
  spf: true
hosts:
- cert_expires: Oct 16 23:13:43 2026 GMT
  host: www.cozy.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cozy Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cozy Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cozy Finance
provider_slug: cozy-finance
slug: cozy-finance-domain-security
source_filename: cozy-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cozy.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:13:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cozy.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cozy-finance/refs/heads/main/security/cozy-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi
- Risk Management
- Smart Contracts
- Ethereum
- Insurance
- Blockchain
- Web3
---
