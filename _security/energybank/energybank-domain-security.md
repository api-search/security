---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: energybank.nz
  spf: true
hosts:
- cert_expires: Oct  4 12:05:01 2026 GMT
  host: www.energybank.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Energybank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnergyBank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EnergyBank
provider_slug: energybank
slug: energybank-domain-security
source_filename: energybank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energybank.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:05:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: energybank.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energybank/refs/heads/main/security/energybank-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Energy Storage
- Offshore Wind
- Renewable Energy
- Data Centers
- Deep Tech
- New Zealand
---
