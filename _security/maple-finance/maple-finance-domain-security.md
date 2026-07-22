---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: maple.finance
  spf: true
hosts:
- cert_expires: Oct 11 21:28:53 2026 GMT
  host: maple.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maple Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maple Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Maple Finance
provider_slug: maple-finance
slug: maple-finance-domain-security
source_filename: maple-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maple.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maple.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maple-finance/refs/heads/main/security/maple-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi Lending
- DeFi
- Onchain Asset Management
- Institutional Lending
- Stablecoin Yield
- Ethereum
- SDK
- MCP
---
