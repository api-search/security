---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quantilia.com
  spf: true
hosts:
- cert_expires: Jan  7 15:21:45 2027 GMT
  host: www.quantilia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantilia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantilia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quantilia
provider_slug: quantilia
slug: quantilia-domain-security
source_filename: quantilia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantilia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:21:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quantilia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantilia/refs/heads/main/security/quantilia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Financial Data
- Portfolio Reporting
- Investment Management
- Asset Management
- Risk Analytics
- ESG
- Private Markets
- Regulatory Reporting
- Data Aggregation
- France
---
