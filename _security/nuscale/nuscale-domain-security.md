---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nuscalepower.com
  spf: true
hosts:
- cert_expires: Sep 20 01:30:35 2026 GMT
  host: www.nuscalepower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NuScale Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NuScale Power
provider_slug: nuscale
slug: nuscale-domain-security
source_filename: nuscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nuscalepower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:30:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nuscalepower.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuscale/refs/heads/main/security/nuscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Nuclear
- Small Modular Reactor
- SMR
- VOYGR
- NuScale Power Module
- US460
- Light Water Reactor
- Passive Safety
- Carbon Free Energy
- Clean Energy
- Energy
- Utilities
- Data Center Power
- Hydrogen
- Desalination
- Process Heat
- Hardware
---
