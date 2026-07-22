---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: networth.mx
  spf: true
hosts:
- cert_expires: Oct 14 00:44:11 2026 GMT
  host: networth.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Net Worth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Net Worth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Net Worth
provider_slug: net-worth
slug: net-worth-domain-security
source_filename: net-worth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: networth.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: networth.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/net-worth/refs/heads/main/security/net-worth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Retirement
- Financial Planning
- Wealth Management
- Insurance
- Mexico
- Investment
---
