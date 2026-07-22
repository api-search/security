---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfs.energy
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: cfs.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commonwealth Fusion Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth Fusion Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Commonwealth Fusion Systems
provider_slug: commonwealth-fusion-systems
slug: commonwealth-fusion-systems-domain-security
source_filename: commonwealth-fusion-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfs.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cfs.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-fusion-systems/refs/heads/main/security/commonwealth-fusion-systems-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fusion Energy
- Tokamak
- SPARC
- ARC
- HTS Magnets
- High-Temperature Superconductors
- REBCO
- Clean Energy
- MIT
- Devens
- Chesterfield County
- Dominion Energy
---
