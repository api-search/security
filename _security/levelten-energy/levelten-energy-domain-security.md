---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leveltenenergy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: levelten.energy
  spf: true
hosts:
- cert_expires: Sep 30 18:05:00 2026 GMT
  host: leveltenenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:52:38 2026 GMT
  host: marketplace.levelten.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 06:58:01 2026 GMT
  host: api.levelten.energy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levelten Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LevelTen Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LevelTen Energy
provider_slug: levelten-energy
slug: levelten-energy-domain-security
source_filename: levelten-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leveltenenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:05:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: marketplace.levelten.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:52:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.levelten.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:58:01 2026 GMT\n  hsts: null\ndomains:\n- domain: leveltenenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: levelten.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levelten-energy/refs/heads/main/security/levelten-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Renewable Energy
- Power Purchase Agreements
- Marketplace
- Clean Energy
- Market Intelligence
- Sustainability
- Carbon
---
