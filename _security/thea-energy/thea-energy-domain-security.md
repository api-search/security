---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thea.energy
  spf: true
hosts:
- cert_expires: Sep 24 02:46:42 2026 GMT
  host: thea.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thea Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thea Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Thea Energy
provider_slug: thea-energy
slug: thea-energy-domain-security
source_filename: thea-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thea.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thea.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thea-energy/refs/heads/main/security/thea-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Fusion Energy
- Nuclear Fusion
- Stellarator
- Clean Energy
- Scientific Computing
- Simulation
- Open Source
- Deep Tech
- New Jersey
---
