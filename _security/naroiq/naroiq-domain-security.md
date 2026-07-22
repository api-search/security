---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: naroiq.com
  spf: true
hosts:
- cert_expires: Sep 29 11:14:19 2026 GMT
  host: www.naroiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Naroiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NaroIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NaroIQ
provider_slug: naroiq
slug: naroiq-domain-security
source_filename: naroiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.naroiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:14:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: naroiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naroiq/refs/heads/main/security/naroiq-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- ETF
- Exchange-Traded Funds
- Fund Infrastructure
- Asset Management
- Financial Services
- Fintech
- Indexing
- Regulatory Compliance
- Europe
---
