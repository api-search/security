---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: powerledger.io
  spf: true
hosts:
- cert_expires: Nov  8 17:32:31 2026 GMT
  host: powerledger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Power Ledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Powerledger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Powerledger
provider_slug: power-ledger
slug: power-ledger-domain-security
source_filename: power-ledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powerledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 17:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powerledger.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-ledger/refs/heads/main/security/power-ledger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Renewable Energy
- Energy Trading
- Environmental Commodities
- Renewable Energy Certificates
- Blockchain
- Sustainability
- Utilities
- Carbon
- Australia
---
