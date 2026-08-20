---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evertas.com
  spf: true
hosts:
- cert_expires: Nov  2 20:25:30 2026 GMT
  host: evertas.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evertas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evertas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evertas
provider_slug: evertas
slug: evertas-domain-security
source_filename: evertas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evertas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 20:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: evertas.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evertas/refs/heads/main/security/evertas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Cryptocurrency
- Digital Assets
- Risk Management
- Underwriting
- Financial-Services
- Blockchain
---
