---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cellcentric.net
  spf: true
hosts:
- cert_expires: Dec 20 15:14:58 2026 GMT
  host: www.cellcentric.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellcentric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellcentric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cellcentric
provider_slug: cellcentric
slug: cellcentric-domain-security
source_filename: cellcentric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cellcentric.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 15:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cellcentric.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellcentric/refs/heads/main/security/cellcentric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fuel Cells
- Heavy‑Duty Trucks
- Hydrogen Powertrain
- OEMs
- Fleet Operators
- Stationary Power
---
