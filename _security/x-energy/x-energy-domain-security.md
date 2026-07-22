---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: x-energy.com
  spf: true
hosts:
- cert_expires: Aug 14 16:09:26 2026 GMT
  host: x-energy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: X Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X-energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: X-energy
provider_slug: x-energy
slug: x-energy-domain-security
source_filename: x-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 16:09:26 2026 GMT\n  hsts: false\ndomains:\n- domain: x-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x-energy/refs/heads/main/security/x-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nuclear Energy
- Small Modular Reactor
- SMR
- High-Temperature Gas Reactor
- HTGR
- Xe-100
- TRISO Fuel
- TRISO-X
- Advanced Reactor
- Clean Energy
- Process Heat
- Industrial Decarbonization
---
