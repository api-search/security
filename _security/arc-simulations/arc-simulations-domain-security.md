---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arcsim.io
  spf: true
hosts:
- cert_expires: Oct 15 09:08:08 2026 GMT
  host: arcsim.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arc Simulations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arc Simulations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arc Simulations
provider_slug: arc-simulations
slug: arc-simulations-domain-security
source_filename: arc-simulations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcsim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 09:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arcsim.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arc-simulations/refs/heads/main/security/arc-simulations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Sports Technology
- Cricket
- Ball Tracking
- Simulation
- Analytics
- Performance Analytics
- Techstars
---
