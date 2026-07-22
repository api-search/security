---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alvaenergy.io
  spf: true
hosts:
- cert_expires: Aug 28 09:11:04 2026 GMT
  host: alvaenergy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alva Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alva Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alva Energy
provider_slug: alva-energy
slug: alva-energy-domain-security
source_filename: alva-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alvaenergy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alvaenergy.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alva-energy/refs/heads/main/security/alva-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy Transition
- Nuclear
- Clean Energy
- Nuclear Uprates
- Power Generation
- Energy
---
