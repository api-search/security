---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solovis.com
  spf: true
hosts:
- cert_expires: Oct  6 20:08:23 2026 GMT
  host: solovis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solovis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solovis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solovis
provider_slug: solovis
slug: solovis-domain-security
source_filename: solovis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solovis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:08:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: solovis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solovis/refs/heads/main/security/solovis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Investment Analytics
- Portfolio Management
- Risk Analytics
- Institutional Investors
- Asset Allocation
- Multi-Asset
- Financial Data
- Reporting
---
