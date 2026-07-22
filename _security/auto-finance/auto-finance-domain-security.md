---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: auto.finance
  spf: true
hosts:
- cert_expires: Aug 18 20:34:24 2026 GMT
  host: app.auto.finance
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auto Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auto Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Auto Finance
provider_slug: auto-finance
slug: auto-finance-domain-security
source_filename: auto-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.auto.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 20:34:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: auto.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto-finance/refs/heads/main/security/auto-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi
- Yield Optimization
- Liquidity Management
- Vaults
- Staking
- Ethereum
- Web3
---
