---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moneytor.in
  spf: true
hosts:
- cert_expires: Sep 21 15:14:30 2026 GMT
  host: moneytor.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aggra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aggra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aggra
provider_slug: aggra
slug: aggra-domain-security
source_filename: aggra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneytor.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:14:30 2026 GMT\n  hsts: false\ndomains:\n- domain: moneytor.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aggra/refs/heads/main/security/aggra-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Debt Collection
- Lending
- Collections
- SaaS
- Machine Learning
- India
---
