---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vanguard.com
  spf: true
hosts:
- cert_expires: Sep 21 23:06:50 2026 GMT
  host: investor.vanguard.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  5 17:56:37 2026 GMT
  host: corporate.vanguard.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanguard Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Vanguard Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Vanguard Group
provider_slug: vanguard-group
slug: vanguard-group-domain-security
source_filename: vanguard-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: investor.vanguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:06:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: corporate.vanguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 17:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: vanguard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanguard-group/refs/heads/main/security/vanguard-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Active Management
- Advisor Services
- Asset Management
- Brokerage
- ETFs
- Finance
- Financial Services
- Fixed Income
- Index Investing
- Institutional Investment
- Investment Management
- Money Management
- Mutual Funds
- Personal Advice
- Recordkeeping
- Retirement
- Wealth Management
---
