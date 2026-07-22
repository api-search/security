---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: current.com
  spf: true
hosts:
- cert_expires: Sep 24 11:38:37 2026 GMT
  host: current.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Current Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Current, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Current
provider_slug: current
slug: current-domain-security
source_filename: current-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: current.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: current.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/current/refs/heads/main/security/current-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Neobank
- Consumer Banking
- Personal Finance
- Payments
- Credit Building
- Savings
- Mobile Banking
---
